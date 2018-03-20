---
published: true
layout: post
title: >-
  Facebook, Cambridge Analytica, And Knowing What API Consumers Are Doing With
  Our Data
date: 2018-03-19T09:00:00.000Z
tags:
  - API Evangelist
  - Observability
  - Social
  - Management
  - Data
  - Privacy
  - Transparency
image: >-
  http://kinlane-productions.s3.amazonaws.com/algorotoscope/builder/filtered/80_140_800_500_0_max_0_-5_-5.jpg
---
I'm processing [the recent announcement by Facebook to shut off the access of Cambridge Analytica](https://newsroom.fb.com/news/2018/03/suspending-cambridge-analytica/) to it's valuable social data. The story emphasizes the importance of real time awareness and response to API consumers at the API management level, as well as the difficulty in ensuring that API consumers are doing what they should be with the data and content being made available via APIs. Access to platforms using APIs is more art than science, but there are some proven ways to help mitigate serious abuses, and identify the bad actors early on, and prevent their operation within the community.

While I applaud Facebook's response, I'm guessing they could have taken more action earlier on. Their response is more about damage control to their reputation, after the fact, than it is about preventing the problem from happening. Facebook most likely had plenty of warning signs regarding what Aleksandr Kogan, Strategic Communication Laboratories (SCL), including their political data analytics firm, Cambridge Analytica, were up to. If they weren't than that is a problem in itself, and Facebook should be investing in more policing of their API consumers activity, as they claim they are doing in their release.

If Aleksandr Kogan has that many OAuth tokens for Facebook users, then Facebook should be up in his business, better understanding what he is doing, where his money comes from, and who is partners are. I'm guessing Facebook probably had more knowledge, but because it drove traffic, generated ad revenue, and was in alignment with their business model, it wasn't a problem. They were willing to look the other way with the data sharing that was occurring, until it became a wider problem for the election, our democracy, and in the press. Facebook should have more awareness, oversight, and enforcement at the API management layer of their platform.

This situation I think highlights another problem of doing APIs, and ensuring API consumers are behaving appropriately with the data, content, and algorithms they are accessing. It can be tough to police what a developer does with data once they've pulled from an API. Where they store it, and who they share it with. You just can't trust that all developers will have the platform, and it's end-users best interest in mind. Once the data has left the nest, you really don't have much control over what happens with it. There are ways you can identify unhealthy patterns of consumption via the API management layer, but Aleksandr Kogan's quizzes probably would appear as a normal application pattern, with no clear signs of the relationships, and data sharing going on behind the scenes.

While I sympathize with Facebook's struggle to police what people do with their data, I also know they haven't invested in API management as much as they should have, and they are more than willing to overlook bad behavior when it supports their bottom line. The culture of the tech space supports and incentivizes this type of bad behavior from platforms, as well as consumers like Cambridge Analytica. This is something that regulations like GDPR out of the EU is looking to correct, but the culture in the United States is all about exploitation at this level, that is until it becomes front page news, then of course you act concerned, and begin acting accordingly. The app, big data, and API economy runs on the generating, consuming, buying, and selling of people's data, and this type of practice isn't going to go away anytime soon.

As Facebook states, they are taking measures to reign in bad actors in their developer community by being more strict in [their application review process](https://www.facebook.com/help/792552774106866). I agree, [a healthy application review process is an important aspect of API management](http://apievangelist.com/2018/02/15/some-common-features-of-an-api-application-review-process/). However, this does not address the regular review of applications usage at the API management level, assessing their consumption as they accumulate access tokens, to more user's data, and go viral. I'd like to have more visibility into how Facebook will be regularly reviewing, assessing, and auditing applications. I'd even go so far as [requiring more observability into ALL applications that are using the Facebook API, providing a community directory that will encourage transparency around what people are building](http://apievangelist.com/2018/03/01/an-observable-industry-level-directory-of-api-providers-and-consumers/). I know that sounds crazy from a platform perspective, but it isn't, and would actually force Facebook to know their customers.

If platforms truly want to address this problem they will embrace more observability around what is happening in their API communities. They would allow certified and verified researchers and auditors to get at application level consumption data available at the API management layer. I'm sorry y'all, self-regulation isn't going to cut it here. We need independent 3rd party access at the platform API level to better understand what is happening, otherwise we'll only see platform action after problems occur, and when major news stories are published. This is the beauty / ugliness of APIs. The cats out of the bag, and platforms need them to innovate, deliver resources to web, mobile, and device applications, as well as remain competitive. APIs also provide the opportunity to peek behind the curtain, and better understand what is happening, and profile the good and the bad actors within each ecosystem--let's take advantage of the good here, to help regulate the bad.
