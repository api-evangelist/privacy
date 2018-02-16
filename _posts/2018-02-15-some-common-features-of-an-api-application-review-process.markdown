---
published: true
layout: post
title: Some Common Features Of An API Application Review Process
date: 2018-02-15T09:00:00.000Z
tags:
  - API Evangelist
  - Applications
  - On-boarding
  - Management
  - SDK
  - Privacy
  - Terms of Service
  - Security
image: ''
---
<p><a href="https://twitter.com/ktinboulder/status/961601920887607296"><img src="https://s3.amazonaws.com/kinlane-productions/kelly-taylor-app-approval-tweet.png" align="right" width="40%" style="padding: 15px;" /></a></p>[I received a tweet from my friend Kelly Taylor with USDS](https://twitter.com/ktinboulder/status/961601920887607296), asking for any information regarding establishing an "approve access to production data" for developers. [He is working on an OAuth + FHIR implementation for the Centers for Medicare and Medicaid Services (CMS) Blue Button API](https://bluebutton.cms.gov/developers/). Establishing a standard approach for on-boarding developers into a production environment always makes sense, as you don't want to give access to sensitive information without making sure the company, developer, and application has been thoroughly vetted.

As I do with my work, I wanted to think through some of the approaches I've come across in my research, and share some tips and best practices. [The Blue Button API team has a section published regarding how to get your application approved](https://bluebutton.cms.gov/developers/#production-api-access), but I wanted to see if I can expand on, while also helping share this information with other readers. This is a relevant use case that I see come up regularly in healthcare, financial, education, and other mainstream industries.

**Virtualization & Sandbox**
The application approval conversation usually begins with ALL new developers being required to work with a sandboxed set of APIs, only providing production API access to approved developers. This requires having a complete set of virtualized APIs, mimicking exactly what would be used in production, but in a much safer, protected environment. One of the most important aspects of this virtualized environment is that there also needs to be robust sets of virtualized data, providing as much parity regarding what developers will experience when they enter the production environment. The sandbox environment needs to be as robust and reliable as the production, which is a mistake I see made over and over from providers, where the sandbox isn't reliable, or as functional, and developers never are able to reach production status in a consistent and reliable way.

**Doing a Background Check**
Next, as reflected in the Blue Button teams approach, you should be profiling the company and organization, as well as the individual behind each application. [You see company's like Best Buy refusing any API signup that doesn't have an official company domain that can be verified](http://apievangelist.com/2016/03/30/best-buy-will-not-issue-api-keys-to-free-email-accounts-and-wants-to-get-to-know-your-company/). In addition to requiring developers provide a thorough amount of information about who they are, and who they work for, many API providers are using background and profiling services like [Clearbit](https://clearbit.com/) to obtain more details about a user based upon their email, IP address, and company domain. Enabling different types of access to API resources depending on the level of scrutiny a developer is put under. I've seen this level of scrutiny go all the way up to requiring the scanning of drivers license, and providing corporate documents before production access is approved.

**Purpose of Application**
One of the most common filtering approaches I've seen centers around asking developer about the purpose of their application. The more detail the better. As we've seen from companies like Twitter, the API provider holds a lot of power when it comes to deciding what types of applications will get built, and it is up to the developer to pitch the platform, and convince them that their application will serve the mission of the organization, as well as any stakeholders, and end-users who will be leveraging the application. This process can really be a great filter for making sure developers think through what they are building, requiring them to put forth a coherent proposal, otherwise they will not be able to get full access to resources. This part of the process should be conducted early on in the application submission process, reducing frustrations for developers if their application is denied.

**Syncing The Legal Department**
Also reflected in the Blue Button team's approach is the syncing of the legal aspects of operating an API platform, and it's applications. Making sure the application's terms of service, privacy, security, cookie, branding, and other policies are in alignment with the platform. One good way of doing this is offering a white label edition of the platforms legal documents for use by the each application. Doing the heavy legal work for the application developers, while also making sure they are in sync when it comes to the legal details. Providing legal develop kits (LDK) will grow in prominence in the future, just like providing software development kits (SDK), helping streamline the legalities of operating a safe and secure API platform, with a wealth of applications in its service.

**Live or Virtual Presentation**
Beyond the initial pitch selling an API provider on the concept of an application, I've seen many providers require an in-person, or virtual demo of the working application before it can be added to a production environment, and included in the application gallery. It can be tough for platform providers to test drive each application, so making the application owners do the hard work of demonstrating what an application does, and walking through all of its features is pretty common. I've participated on several judging panels that operate quarterly application reviews, as well as part of specific events, hackathons, and application challenges. Making demos a regular part of the application lifecycle is easier to do when you have dedicated resources in place, with a process to govern how it will all work in recurring batches, or on a set schedule.

**Getting Into The Code**
As part of the application review process many API providers require that you actually submit your code for review via Github. Providing details on ALL dependencies, and performing code, dependency, and security scans before an application can be approved. I've also see this go as far as requiring the use of specific SDKs, frameworks, or include proxies within the client layer, and requiring all HTTP calls be logged as part of production applications. This process can be extended to include all cloud and SaaS solutions involved, limiting where compute, storage, and other resources can be operated. Requiring all 3rd party APIs in use be approved, or already on a white list of API providers before they can be put to use. This is obviously the most costly part of the application review process, but depending on how high the bar is being set, it is one that many providers will decide to invest in, ensuring the quality of all applications that run in a production environment.

<p><img src="https://s3.amazonaws.com/kinlane-productions/apple-app-review.png" align="right" width="40%" style="padding: 15px;" /></p>

**Regular Review & Reporting**
One important thing about the application review process is that it isn't a one time process. Even once an application is accepted an added into the production environment, this process will need to be repeated for each version release of the application, along with the changes to the API. Of course the renewal process might be shorter than the initial approval workflow, but auditing and regular check-in should be common, and not forgotten. This touches on the client level SDK, and API management logging needs of the platform, and that regular reporting upon application usage and activity should be available in real time, as well as part of each application renewal. API operations is always about taking advantage the real time awareness introduced at the API consumption layer, and staying in tune with the healthy, and not so healthy patterns that emerge from logging everything an application is doing.

**Business Model**
It is common to ask application developers about their business model. The absence of a business model almost always reflects the underlying exploitation and sale of data being access or generated as part of application's operation. Asking developers how they will make money and sustain their operations, along with regular checkins to make sure it is truly in effect, is an easy to ensure that applications are protecting the interests of the platform, its partners, and the applications end-users.

There are many other approaches I've seen API providers require before accepting an application into production. However, I think we should also be working hard to keep the process simple, and meaningful. Of course, we want a high bar for quality, but as with everything in the API world, there will always be compromises in how we deliver on the ground. Depending on the industry you are operating the bar will be made higher, or possibly lowered a little to allow for more innovation. I've included a list of some of the application review process I found across my research--showing a wide range of approaches across API providers we are all familiar with. Hopefully that helps you think through the application review process a little more. It is something I'll write about again in the future as I push forward my research, and distill down more of the common building blocks I'm seeing across the API landscape.

**Some Leading Application Review Processes**

- [Instagram](https://www.instagram.com/developer/review/)
- [SAP Concur](https://developer.concur.com/manage-apps/app-certification.html)
- [Paypal](https://developer.paypal.com/docs/classic/lifecycle/goingLive/)
- [Adsense](https://developers.google.com/adsense/host/review_main)
- [Shopify](https://help.shopify.com/api/listing-in-the-app-store/app-requirements-and-success-criteria/app-review-checklist)
- [Riot Games](https://developer.riotgames.com/application-process.html)
- [Slack](https://api.slack.com/security-review)
- [Docusign](https://www.docusign.com/blog/dsdev-docusign-go-live-process-now-automated/)
- [Splunk](http://dev.splunk.com/view/app-cert/SP-CAAAE8P)
- [Ebay](https://go.developer.ebay.com/compatible-application-check-and-checklist-going-live)
- [Apple](https://developer.apple.com/app-store/review/)
