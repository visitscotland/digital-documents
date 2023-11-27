# Digital Partner Standards VisitScotland

Last edited: 21 November 2023

- [Digital Partner Standards VisitScotland](#digital-partner-standards-visitscotland)
  - [Introduction](#introduction)
  - [Types of solution](#types-of-solution)
    - [Product Type Systems](#product-type-systems)
    - [Custom Digital Assets](#custom-digital-assets)
  - [Processes](#processes)
  - [Management and approval sign off for creative digital briefs](#management-and-approval-sign-off-for-creative-digital-briefs)
    - [Briefing a Digital Partner](#briefing-a-digital-partner)
    - [Proposed Technical Implementation](#proposed-technical-implementation)
    - [Quote and Statement of work](#quote-and-statement-of-work)
    - [Approval to proceed](#approval-to-proceed)
    - [Proof of concept](#proof-of-concept)
    - [Implementation phase](#implementation-phase)
    - [VisitScotland’s Architectural Roadmap and Platforms](#visitscotlands-architectural-roadmap-and-platforms)
  - [Appendix](#appendix)
    - [Coding Standards](#coding-standards)
    - [Source Control](#source-control)
    - [Version Control](#version-control)
    - [Security Standards](#security-standards)
    - [Supported Platforms](#supported-platforms)
    - [Browsers, Operating Systems and Mobile Platforms](#browsers-operating-systems-and-mobile-platforms)
    - [Responsive Design](#responsive-design)
    - [Logging Principles and Standards](#logging-principles-and-standards)
    - [VisitScotland Software development Cybersecurity Standards](#visitscotland-software-development-cybersecurity-standards)
    - [Supply Chain Compromise](#supply-chain-compromise)
    - [Maintenance Policy](#maintenance-policy)
    - [Accessibility](#accessibility)
    - [Readability](#readability)
    - [Progressive Enhancement](#progressive-enhancement)
    - [Analytics, SEO and GDPR](#analytics-seo-and-gdpr)
      - [Tracking requirements](#tracking-requirements)
      - [Reporting requirements](#reporting-requirements)
    - [GPDR compliance in the use of cookies and similar technologies](#gpdr-compliance-in-the-use-of-cookies-and-similar-technologies)
    - [Data collection on forms](#data-collection-on-forms)
    - [SEO Basic Checklist](#seo-basic-checklist)
    - [Quality Assurance](#quality-assurance)

## Introduction

VisitScotland’s consumer and corporate websites are at the heart of driving, and supporting, the tourism industry. As a public sector body, we are committed to the delivery of high quality, accessible assets which serve all our users. Our websites are populated by assets delivered inhouse and digital partner agencies. This document details our standards and expectations for seamlessly integrating our digital deliverables.

VisitScotland has a duty to build sites and digital content in a secure, accessible and cost-effective manner in line with internal development, security, information security, accessibility standards along with [Digital Scotland Service Standard](https://www.gov.scot/publications/digital-scotland-service-standard/) as set out by the Scottish Government and the UK Government

[All public sector assets must conform to WCAG 2.2 AA accessibility standards.](https://www.gov.uk/guidance/accessibility-requirements-for-public-sector-websites-and-apps)

This document ties in with VisitScotland’s Digital Accessibility Standards document.

## Types of solution

### Product Type Systems

Standalone assets are hosted, supported and deployed completely separately from any VisitScotland support or maintenance. Normally these systems are termed “out of the box” solutions where it is quicker or more cost effective to buy in a product.

Before purchasing these systems, approval will be required via the VisitScotland Architecture and Design Board (ADB). Normally these products will be delivered via a project and procurement process. Standard project controls will be in place to look after delivery and lifecycle considerations of these systems.

The long-term future of these systems should be considered at the outset along with any longer term architectural and VisitScotland support considerations, including options on hosting and maintenance costs. Broadly speaking, these projects extend beyond a 10-day delivery period.

VisitScotland’s procurement acquisition cycles typically run for three years following successful initial tender.

Some assets purchased out with the organisation may have a longer lifespan. All briefs need to consider how this requirement will be supported, maintained, and budgeted for. Alternatively, retirement should be considered as a viable option depending on success metrics and performance of the system in question and should be queried during briefing stage. Many event campaign sites fall under this temporary lifecycle (for example Cycling World Championships) and plans for retiral should be included in any tender documentation along with associated costs and backup processes.

### Custom Digital Assets

A range of custom digital assets are produced by internal teams and external suppliers in partnership. VisitScotland will discuss options on how a digital asset can be developed and encourage digital partners to work to architectural guidelines when developing these.

All custom digital development should adhere as closely as possible to VisitScotland development processes, practices and standards, as laid out in this document.

## Processes

When developing custom assets, VisitScotland follows general industry standards and best practice in relation to Agile development. Some of the fundamental items expected as part of this are:

- Adopting Agile/Lean methodologies that encourages incremental feedback, such as Showcases etc. Early engagement in this process with relevant VisitScotland teams is vital so that items are delivered to correct specification and quality.

- Proactive understanding and engagement with relevant teams both technical and marketing led.

- Access to source code, build and deployment artefacts with an updated changelog.

- Provision of and/or access to support applications, such as availability APIs for monitoring and support.

- Scheduling of assets to fit with VisitScotland’s digital team’s sprint cycles and programme of work.

Whilst promoting swift and iterative asset development, VisitScotland requires that this is conducted in conjunction with an appropriate level of governance and documentation. It is a requirement that there be sign off from the VisitScotland Digital team for any digital assets that will be accessed via any VisitScotland website or delivered from a VisitScotland system. Recognising that this is a risk-based approach, it should be noted that any asset that is procured by VisitScotland has the potential to cause regulatory or reputational damage.

All custom digital assets must consider or comply with VisitScotland practices, in terms of:

- VisitScotland Development & Cyber-security standards.

- UX standards, including digital accessibility.

- Analytics, SEO and GDPR requirements.

- QA / Testing policies.

## Management and approval sign off for creative digital briefs

### Briefing a Digital Partner

The creative team owning the partnership will put together a brief with the Digital Partner that references this Digital Standards documentation. The brief will also be sent to product owners for .com and .org for cascading to functional teams for review.

If there is a need to deviate from standards, then the recommended delivery architecture should be discussed with VisitScotland’s Digital team prior to submission of the Proposed Technical Implementation.

### Proposed Technical Implementation

The proposed technical implementation will be signed of via VisitScotland’s Architecture and Design Board (ADB)

### Quote and Statement of work

The Digital Partner will provide a quote for the brief which will include an implementation plan, a testing plan and deployment plan.

### Approval to proceed

Sign off from both the creative owner and technical owner can then be given in collaboration

### Proof of concept

If required, a proof of concept should be provided and delivered to VisitScotland for review and approval.

### Implementation phase

During the implementation phase all Design, Development, UX, SEO and Content creation will take place along with all testing (including accessibility) and bug fixing. This should be done in an iterative process where VisitScotland will be regularly “Showcased” progress. It may be necessary to conduct daily “stand up” ceremonies with VisitScotland to track progress and share information.

### VisitScotland’s Architectural Roadmap and Platforms

VisitScotland provides platforms that are open and can be integrated into, preferably Digital Partners would develop a solution using one of:

- VisitScotland APIs
- CMS (Bloomreach BRXM)
- Dynamics CRMs
- SharePoint
- Marketing Automation Platform
- Object stores such as Elastic Search or MongoDB.

Producing assets that are sympathetic to VisitScotland systems will enable reuse and make maintenance of future assets simpler and may, over an asset’s lifecycle, reduce cost.

Our CMS, Bloomreach BRXM is a document-based CMS that allows the rendering of content documents via a headless API. The preference is that all content is stored within this CMS platform - rendering can be achieved via this system or via APIs onto third party systems.

Where appropriate, all assets should consider the creation of APIs to allow integration if required by VisitScotland.

## Appendix

### Coding Standards

In general, coding standards will be enforced via Linting and Static Analysis Tools configured within the developers IDE and will also be analysed when code is checked into source control as part of a development pipeline.

The development team in VisitScotland will agree on a defined set of rules that can be configured for relevant IDEs and source control scanning tools.

Static analysis standards configuration can be shared with partner organisations by requesting access to the developer environment configuration repository (GitHub account required to grant access).

### Source Control

VisitScotland digital developers will use GitHub as the source control system and follow Gitflow as the method of implementing source control.

### Version Control

VisitScotland digital developers will utilise relevant version control as part of their build and release processes.

A custom data-version attribute should be included in the page source of any digital asset that shows not only the version number of the asset but all the build date and time in the following format:

- data-version="1.0.34 (23266150223)"

where *23266150223* represents a time of: 15:02:23 on the 266th day of the year 2023.

### Security Standards

VisitScotland’s policies on Security standards are under review, however standard [OWASP principles](https://owasp.org/) along with the Cyber Security standards laid out in this document should be followed.

### Supported Platforms

VisitScotland development standards and the platforms supported are reviewed on a quarterly basis.

Each project should be assessed on a case-by-case basis considering the target audience groups and any relevant technologies or product changes in the marketplace since the date of this document. Analytics should be used to specify the Operating Systems, Browser and Versions etc used to view VisitScotland digital assets.

A single baseline standard should be applied across all development though it is likely that variations in target audiences and devices will alter what is supported and therefore tested against.

Such a standard baseline is outline in the following sections.

### Browsers, Operating Systems and Mobile Platforms

As a minimum, the following browsers should be supported for any new digital web asset:

| OS            | Browser       | Version |
| ------------- | ------------- | ------- |
| Windows           | Google Chrome     |Current Version |
|                   | Mozilla Firefox   | Current version + ESR (Extended Support Release) |
|                   | Microsoft Edge    | Current Version
| macOS             | Safari            | Current Version
|                   | Google Chrome     | Current Version
|                   | Mozilla Firefox   | Current Version + ESR (Extended Support Release)
| iOS               | Safari            | Current Version
| Android           | Google Chrome     | Current Version
|                   | Samsung Internet  | Current Version

As a minimum, the following operating systems or platforms should be supported:

| OS        | Version                               |
|---------- |---------------------------------------|
| Windows   | 10 & 11                               |
| macOS     | Catalina (2019) onwards               |
| iOS       | current version + one prior           |
| Android   | current version + two versions prior  |

### Responsive Design

All assets must adhere to responsive design principles and thus testing at a variety of viewport sizes is imperative. As a minimum, the following resolutions should be supported for any new Digital Asset:

| Device Category   | Size | Units    |
| ----------------- | --------- | -------- |
| mobile            | 375x667   | Points
| mobile            | 360x640   | Points
| tablet            | 768x1024  | Points
| desktop           | 1366x768  | Pixels
| desktop           | 1920x1080 | Pixels
| mobile            | 320x568   | Points
| mobile            | 360x740   | Points
| mobile            | 414x736   | Points
| desktop           | 1440x900  | Pixels
| mobile            | 375x812   | Points

 These metrics are reviewed regularly.

### Logging Principles and Standards

Appropriate levels of logging should be in place to support fault resolution and application support.

### VisitScotland Software development Cybersecurity Standards

Cybersecurity standards protect VisitScotland, its partners and customers from attacks that could compromise data or damage systems.

In terms of custom developed systems, as well as OWASP principles mentioned in section 5.4, there are a couple of other security vectors that need to be considered below.

### Supply Chain Compromise

Code should be scanned regularly by the partner using library scanners that can detect any life cycle issues such as security vulnerabilities or out of date libraries.  VisitScotland may scan and alert to issues as and when necessary.

### Maintenance Policy

When developing or procuring digital content assets, consideration should be given to their lifecycle. All software will, over time, become less relevant and require maintenance. Inherently as software ages its maintenance becomes more expensive, and it may even become unsupportable due to:

- Obsolescence of the language and libraries that were used to construct it.

- Underlying technology stack, and/or hosting environment, may become unsupportable.

- Standards that it was developed to, such as usability, or cyber security fall behind.

- Consideration of a maintenance phase should be planned and costed for which caters not just for hosting but any functional or technical change to assets.

All digital assets should be introduced such that periodical maintenance reviews take place:

- These should include patching/upgrading any identified security vulnerability.

- Ideally this is an automated system that alerts to security issues found in any code.

### Accessibility

As of 23rd September 2019, all new Public Sector bodies are legally required to ensure their websites and apps are “perceivable, operable, understandable and robust” by complying with WCAG 2.1 Accessibility Guidelines AA Standard. Therefore, all Digital Partners must adhere to current version of VisitScotland's **Digital Accessibility Standards** document when producing any new digital asset, providing any documentation asked for therein.

### Readability

All content will be provided by VisitScotland’s Content team (unless specified) who will quality control the Readability of the content where required, as specified in the project’s creative brief.

### Progressive Enhancement

Progressive enhancement is a strategy in web design that puts emphasis on web content first. This strategy involves separating the presentation semantics from the content, with presentation being implemented in one or more optional layers, activated based on aspects of the browser or Internet connection of the user.

Digital Partners should adopt a progressive enhancement approach to front-end implementation so that any asset caters for scenarios where JavaScript or CSS code fails to load or has been intentionally disabled.

Additional guidance can be found in the [UK Government website on Progressive Enhancement](https://www.gov.uk/service-manual/technology/using-progressive-enhancement).

Further, where JavaScript frameworks are chosen to build client-side web applications, consideration should be given to mitigate problems between client and server and address accessibility, performance, and SEO requirements. To this end Server-Side Rendering implementations maybe required, please speak to VisitScotland’s development team who will be happy to offer advice.

### Analytics, SEO and GDPR

All assets developed for VisitScotland should comply with [Digital Scotland Service Standards](https://www.gov.scot/publications/digital-scotland-service-standard/) and should include VisitScotland’s standards on general analytics, SEO and GDPR.

Discussion with relevant teams should be had early in any Discovery phase and before development starts. Relevancy of the asset should determine how much engagement will be required. Specific requirements on these topics are outlined in the following sections.

In terms of GDPR, for any assets recording identifiable data, Digital Partners should work with the VisitScotland Information Officer to follow established GDPR processes within VisitScotland.

#### Tracking requirements

- Google Tag Manager implementation on websites: This will be used to implement standard tools and technologies including, but not limited to google analytics and tracking technologies for marketing purposes (i.e. Facebook pixel, DoubleClick floodlight tags, LinkedIn analytics pixel, etc).

- DataLayer implementation on the asset with sufficient information to allow tracking of relevant metrics and business KPIs, including but not limited to standard and custom DataLayer variables, unique event IDs, and metadata pushed into the DataLayer.

#### Reporting requirements

The VisitScotland Digital Analytics team will manage the setup of any Analytics infrastructure, with the assistance of any Digital Partner when appropriate. As stated above, discussions with the Analytics team should be had early in any Discovery phase and before development starts. These discussions are likely to centre around:

- Creation of a Google Analytics account/property/views to ensure accurate and relevant reporting of the asset. This will include standard analytics metrics (pageviews, sessions, bounce rate, etc) as well as specific events tracking, goals and KPIs for the asset.

- Site search tracking and reporting within Google Analytics.

- SEO reporting in Google Analytics.

- Custom channel grouping based on specific asset needs.

Note, that website reporting is subject to **opt-in consent** for all non-essential/non-strictly necessary cookies. See GDPR compliance in the use of cookies and similar technologies for further information.

### GPDR compliance in the use of cookies and similar technologies

To comply with current GDPR legislation, all VisitScotland digital assets (websites and mobile apps) must **obtain consent before collecting any user data, personal or otherwise**. This requires the implementation of opt-in consent for cookies and similar technologies (e.g. google analytics, Facebook pixel, YouTube embedded videos, etc).

All but essential or strictly necessary cookies will require opt-in consent to fire/deploy on a user’s browser. As a result, Digital Partners must consider the impact of intended / required functionality if consent for the relevant cookies is not given and mitigate such impacts to the satisfaction of VisitScotland.

To comply with GDPR legislation in the use of cookies, assets must include the following elements:

- Cookie banner: with clear and easy to understand information, the option to accept/manage cookie settings and a link to a detailed cookie policy page where users can access more information about the types of cookies used on the site (including cookie provider, name, purpose, category and lifespan).

- Cookie preference centre: where users can select/view/manage their cookie preferences. This must be easily accessible on an asset at any point during the user journey. e.g. through a link on the footer of a web page.

- Cookie policy page: in clear / plain language regarding the use of cookies, a list of current cookies used on the website and access to the preference centre through a link or button. See <www.visitscotland.org> for reference.

Fallbacks: in certain instances, a website feature or functionality will require explicit consent to be activated on the website (i.e. YouTube videos). If users do not provide consent for the relevant cookie category, said content or functionality will not work correctly. In these cases, a fallback should be added to the relevant modules/widgets to inform users and give them the option to modify their cookie settings to access the relevant content and improve user experience. See below examples of fallbacks for <www.visitscotland.com>.

Digital Partners are advised to use the <www.visitscotland.com> or <www.visitscotland.org> websites for reference.

The criteria stated above must be applied to all elements of any asset including subdomains and any additional functionality added in subsequent phases of the asset’s lifespan.

The cookie banner and preference centre must adhere to the latest version of VisitScotland’s Digital Accessibility Standards document.

In order to remain compliant, any asset is expected to be flexible and scalable to quickly accommodate any future changes in legislation.

When required/appropriate, VisitScotland may choose to implement OneTrust cookie consent software to meet the above requirements. In these cases, the implementation will be managed by the Digital Analytics team via Google Tag Manager in collaboration with internal development teams and/or Digital Partner.

The information outlined in this section refers to current GDPR legislation in the use of cookies and similar website and app technologies (pixels, mobile and in app tracking technologies) only and it does not cover wider GDPR and other legal requirements such as forms or payment data. As stated previously, for any assets recording identifiable data, Digital Partners should work with the VisitScotland Information Officer to follow established GDPR processes within VisitScotland.

### Data collection on forms

The following are principles to applied to data collection on forms. Digital Partners should work with the VisitScotland Information Office to establish which apply and have each asset signed off.

- Data should only be collected where necessary and for a specific purpose.

- Fair processing statement must be included at point of data capture. This should outline what VisitScotland intends to do to each piece of data.

- Detailed data policy must also be included.

- Data Protection Policy must reflect what is happening with the data and be open, honest & transparent.

- Explicit consent must be given to receive any type of marketing. This is usually in the form of a tick box; using pre-agreed wording.

- Consent should be split for each channel. This gives users choice.  

- Consent should be explicit for Third Parties / partners and should not be bundled in with VisitScotland. Again, this gives consumers choice.

- Only data from adults will be collected by VisitScotland. This is currently covered in the visitscotland.com terms and conditions.

- Subscribing to marketing must be freely given. Users should not be made to sign-up to marketing in order to complete another transaction.

- Every time personal contact information is captured, the consent question(s) must be asked unless it is recognised that the person is already known.

- The last instruction a person gives must always be followed.

- There is a link between form fields & the data structure so that data can easily be collected and stored against the contact record.

- To maintain data integrity, minimal data capture must be obtained.

- Data should be captured, processed, and passed to VisitScotland as quickly as possible (preferably via API)

- The date and time of a form submission should be captured, along with the response.

### SEO Basic Checklist

The following SEO requirements should be met for any digital asset.

- Keyword Research should be carried out at the beginning of each project to help shape the content ideation process. Keyword research can be provided by the VisitScotland SEO team. Each asset should have a target keyword set where possible.

- Keywords should be threaded naturally into URLs, title tags, meta descriptions, H1s and copy.

- Each page should have a unique Title tag. Title tags should be no longer than 70 characters (including spaces and brand).

- Each page should be assigned a unique meta description. Meta descriptions should be no longer than 160 characters (including spaces).

- All assets should use breadcrumbs, in-line with the relevant VisitScotland property.

- In order to protect against duplicate content issues, self-referencing canonical tags should be implemented on all assets. These should be included in the <head> section of pages. Absolute URLs should be used.

- Each asset should be available from one unique URL only.

- Each asset should have one, unique H1. Where the asset has multiple URLs, each URL should have one, unique H1.

- Creating subdomains, microsites and eBooks should be avoided unless there is a valid reason not to place the asset on an existing VisitScotland property.

- Hreflang tags should be included in the <head> section of pages if the asset is translated.

- All images should have alt text.

- Image file size should be reduced as much as possible to protect page speed.

- Filenames for images should be meaningful, descriptive and clear.

- All assets should link to other relevant VisitScotland content to aid discoverability for users and search engines.

- Ensure use of JavaScript is SEO friendly. Testing should be carried out to ensure that the asset can be crawled, rendered and indexed by search engines.

- All assets should be built mobile first and should be responsive.

- Each page should have open graph mark-up included in the <head> section of the html for social sharing.

- Assets placed on either visitscotland.com or visitscotland.org properties, should not use a trailing slash in the URL(s)

- URLs should be easy to read for users. Shorter URLs are preferable.

### Quality Assurance

Testing and Software Quality Assurance is a key requirement of any digital delivery and is very important to VisitScotland. From a legal and reputational standpoint, Digital Partners are expected to have carried out relevant quality assurance steps when developing assets for VisitScotland. Failure to carry out these steps will result in rework and missed opportunity as well as the above repercussions.

A typical QA process would involve:

- Review of requirements / Acceptance Criteria via Behavioural Driven Development

- Test planning / writing test cases

- Risk based Exploratory testing

- Unit testing via Test Driven Development

- Integration testing

- Accessibility Testing

- System testing

- Performance testing

- Security testing

- Cross-browser testing / cross-platform testing

- Updating test cases

- Regression testing

Automated tests should be utilised wherever possible so that Quality of digital assets can be measured swiftly and in a repeatable fashion against any environment, whether that be a Development, Staging / Acceptance or Production. It should be noted that any QA process adopted should be relevant in terms of the complexity of the asset being delivered.

**Test documentation including Test Summary Reports should be produced as standard and shared with VisitScotland on the delivery of every asset**.
