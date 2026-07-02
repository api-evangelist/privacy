# Privacy (privacy)
An index and topic collection covering privacy management, consent management, data subject rights, data classification, and PII detection APIs. Privacy platforms help organizations comply with global data protection regulations such as GDPR, CCPA/CPRA, LGPD, and PIPL by managing user consent, fulfilling data subject access and deletion requests, building data inventories and processing records, and discovering, classifying, and redacting personal information across applications and data stores. This collection includes enterprise privacy management platforms like OneTrust, consent management platforms (CMPs), PII detection and data discovery services, privacy-preserving vaults and tokenization providers, and the open standards and registries (IAB TCF, Global Privacy Control, W3C DPV) that underpin machine-readable privacy and consent signals on the web.

**URL:** [https://apievangelist.com](https://apievangelist.com)

## Tags:

 - Privacy, Consent Management, Data Subject Rights, GDPR, CCPA, PII Detection, Data Privacy, Cookie Consent

## Timestamps

- **Created:** 2026-05-19
- **Modified:** 2026-05-19

## Common Properties

- [Portal](https://apievangelist.com)
- [GitHubOrganization](https://github.com/api-evangelist)
- [JSONSchema - Consent Record Schema](https://raw.githubusercontent.com/api-evangelist/privacy/refs/heads/main/json-schema/privacy-consent-record-schema.json)
- [JSONSchema - Data Subject Request Schema](https://raw.githubusercontent.com/api-evangelist/privacy/refs/heads/main/json-schema/privacy-data-subject-request-schema.json)
- [JSON-LD](https://raw.githubusercontent.com/api-evangelist/privacy/refs/heads/main/json-ld/privacy-context.jsonld)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/privacy/refs/heads/main/vocabulary/privacy-vocabulary.yaml)

## Features

| Name | Description |
|------|-------------|
| Consent Management | Capture, store, and revoke user consent for cookies, data processing, marketing communications, and third-party data sharing across web, mobile, OTT, and server-side surfaces, in line with IAB TCF, GPC, and regional consent regimes. |
| Data Subject Rights Automation | Intake, identity verification, routing, and fulfillment of data subject access, correction, deletion, portability, and opt-out requests required by GDPR, CCPA/CPRA, LGPD, and similar regulations. |
| PII Detection and Data Discovery | Machine learning and pattern-based discovery, classification, and labeling of personally identifiable information across structured databases, data lakes, file shares, SaaS apps, and unstructured documents. |
| Data Inventory and Records of Processing | Maintain Article 30 records of processing activities, data maps, vendor inventories, and data transfer registers that document where personal data lives and how it flows across systems. |
| Privacy-Preserving Data Vaults | Tokenization, polymorphic encryption, and de-identification services that isolate sensitive personal data behind privacy APIs so applications can operate on tokens or pseudonyms instead of raw PII. |
| Privacy Notices and Preference Centers | Publish and version externally-facing privacy notices, cookie notices, and end-user preference centers so individuals can review and update how their personal data is used. |
| Consent and Opt-Out Signals | Honor and propagate machine-readable web signals such as Global Privacy Control (GPC), Do Not Sell or Share, IAB TCF transparency and consent strings, and Authorized Agent opt-outs across downstream systems. |
| Privacy Compliance Monitoring | Continuous monitoring of cookies, trackers, SDKs, third-party scripts, and data flows to detect privacy regressions, undisclosed processors, and policy violations before they become enforcement events. |

## Use Cases

| Name | Description |
|------|-------------|
| GDPR and CCPA Cookie Consent | Deploy a consent management platform on web and mobile to capture cookie and tracker consent before loading non-essential tags, with audit-grade records of who consented to what and when. |
| Data Subject Access Request Fulfillment | Receive a DSAR via a privacy portal, verify identity, fan out search across CRM, marketing, analytics, and data warehouse systems, and return a packaged response within the regulatory deadline. |
| PII Discovery Across Cloud Storage | Continuously scan S3 buckets, data lakes, and SaaS file shares for unprotected personal data, then automatically classify, label, and route findings to security and privacy teams for remediation. |
| Vendor and Third-Party Risk Assessment | Track third parties processing personal data, send privacy and security questionnaires, store completed assessments, and surface high-risk processors for review and renegotiation. |
| Tokenized Customer Data Platform | Replace direct storage of names, emails, phone numbers, and payment data in downstream systems with vault-issued tokens, so analytics and marketing pipelines can run on de-identified data. |
| Privacy Impact Assessments | Build, review, and version Data Protection Impact Assessments (DPIAs) and Transfer Impact Assessments (TIAs) as part of product launch and data sharing workflows. |
| Opt-Out Signal Honoring | Detect Global Privacy Control and Do Not Sell or Share signals on inbound web traffic and propagate the resulting opt-out state to ad tech, analytics, and CRM systems within the regulatory window. |
| AI and LLM Data Loss Prevention | Detect and redact PII, secrets, and regulated data in prompts and responses flowing through AI assistants and LLM applications, with full audit logs for privacy and security review. |

## Integrations

| Name | Description |
|------|-------------|
| OneTrust | Enterprise privacy, consent, and GRC platform with APIs for privacy management, third-party risk, cookie consent, and certification automation. |
| Nightfall AI | Cloud-native data leak prevention and PII detection API that scans SaaS apps, data stores, and LLM traffic for sensitive data. |
| Amazon Macie | AWS service for discovering and classifying sensitive data such as PII and financial data in S3 using machine learning. |
| LiveRamp | Identity resolution and data collaboration platform with consent, permissioning, and privacy-preserving data sharing APIs. |
| Matomo | Open source, privacy-friendly web analytics platform that supports cookieless tracking and GDPR-compliant analytics deployments. |
| Mixpanel | Product analytics platform with privacy controls, consent integration, and APIs for deletion and access requests. |
| Segment | Customer data platform with consent, privacy, and end-user data deletion APIs integrated across hundreds of destinations. |
| Snowplow | Open source behavioral data platform with consent context, GDPR-aware event collection, and pseudonymization features. |
| Google Tag Manager | Tag management system used as the deployment surface for consent mode, server-side tagging, and downstream CMP signals. |
| GDPR | European Union data protection regulation that sets the global baseline for lawful processing, data subject rights, and cross-border transfers. |
| CCPA | California Consumer Privacy Act and CPRA expansion that establish opt-out, access, deletion, and sensitive personal information rights for California residents. |

## Artifacts

Machine-readable privacy specifications organized by format.

### JSON Schema

- [Consent Record Schema](json-schema/privacy-consent-record-schema.json)
- [Data Subject Request Schema](json-schema/privacy-data-subject-request-schema.json)

### JSON Structure

- [Consent Record Structure](json-structure/privacy-consent-record-structure.json)
- [Data Subject Request Structure](json-structure/privacy-data-subject-request-structure.json)

### JSON-LD

- [Privacy Context](json-ld/privacy-context.jsonld)

## Vocabulary

- [Privacy Vocabulary](vocabulary/privacy-vocabulary.yaml) — Unified taxonomy mapping core resources, actions, workflows, and personas across consent management, data subject rights, PII detection, and data inventory programs

## Network

This index references the following privacy and consent management repositories:

- [OneTrust](https://github.com/api-evangelist/onetrust)
- [Nightfall AI](https://github.com/api-evangelist/nightfall-ai)
- [Amazon Macie](https://github.com/api-evangelist/amazon-macie)
- [LiveRamp](https://github.com/api-evangelist/liveramp)
- [Matomo](https://github.com/api-evangelist/matomo)
- [Umami](https://github.com/api-evangelist/umami)
- [Plausible](https://github.com/api-evangelist/plausible)
- [Swetrix](https://github.com/api-evangelist/swetrix)
- [Pi-hole](https://github.com/api-evangelist/pi-hole)
- [Gen Digital](https://github.com/api-evangelist/gen-digital)
- [Confidential Computing Consortium](https://github.com/api-evangelist/confidential-computing-consortium)
- [Regulatory Templates](https://github.com/api-evangelist/regulatory-templates)
- [Mixpanel](https://github.com/api-evangelist/mixpanel)
- [Snowplow](https://github.com/api-evangelist/snowplow)
- [Segment](https://github.com/api-evangelist/segment)
- [Dead Drop](https://github.com/api-evangelist/dead-drop)
- [Google Tag Manager](https://github.com/api-evangelist/google-tag-manager)
- [Privacy by Design](https://github.com/api-evangelist/privacy-by-design)
- [Data Privacy Standards](https://github.com/api-evangelist/data-privacy-standards)
- [GDPR](https://github.com/api-evangelist/gdpr)
- [CCPA](https://github.com/api-evangelist/ccpa)
- [HIPAA](https://github.com/api-evangelist/hipaa)
- [Customer Database](https://github.com/api-evangelist/customer-database)
- [Disclosure Requirements](https://github.com/api-evangelist/disclosure-requirements)
- [VPN](https://github.com/api-evangelist/vpn)
- [Perf.ai](https://github.com/api-evangelist/perf-ai)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
