---
title: Resources
description: 'What is EMMY?'
permalink: /resources/
layout: layouts/page
section: resources
tags: emmy
eleventyNavigation:
  parent: emmy-resources
  key: emmy-resources-main
  order: 1
  title: What is EMMY?
sidenav: true
sticky_sidenav: true
---

# Eligibility Made Easy (Emmy)

Emmy is suite of open-source tools developed by the Centers for Medicare & Medicaid Services (CMS) that consists of two primary components:

* Emmy application for Medicaid applicants and enrollees to report income, hours worked, education enrollment status, and volunteering activities
* Emmy Application Programming Interface (API) for states to access a centralized hub for data sources to streamline reporting by applicants


Emmy uses consent-based verification (CBV) with multiple data sources, making the process much faster and more efficient than a simple document-upload service. CBV enables additional cost avoidance by optimizing manual document review processes. Rather than having to process incorrect or blurry documents, consent-based verification produces an easily consumed report with essential information. Verification information is returned in a standardized format easy for other systems to process (JSON), allowing integration with existing state systems. 

Emmy is under active development by CMS, with new updates released on a weekly cadence. [Check out the release history](https://github.com/DSACMS/iv-cbv-payroll/releases) on the GitHub repository. By participating now, you can help shape the development of Emmy and ensure it meets your states’ requirements. Most critically, Emmy is planned as a modular tool, allowing states to select which components they wish to use for verification, along with an API service to support state implementations of a custom UI.

### Key Benefits for Applicants

  

|  |  |  |  |
| :-- | :-- | :-- | :-- |
|  | Problem it solves | Emmy feature | Result |
| No working with paper paystubs or organizing your PDFs | Proving income can be a cumbersome process. | The basic design of Emmy is a massive streamlining of the classic income verification process. | Emmy delivers huge savings of time and effort for every users. |
| Cohesive view of education, volunteering, and employment | Applicants who wish to show a combination of volunteering, school, and work often need to add notes, and can't see if their information is complete before its sent to an agency. | Emmy's interface can show applicants which months are covered by the data they've submitted, and whether submission includes the required number of hours. | Applicants are more confident that they're submitting complete applications. |
| Detection of lost jobs | Verifying that a job has ended used to require a phone call to the former employer. | With payroll provider integration, Emmy can detect the loss of a job without special representative attention. | A much easier process for state agencies and applicants. |
| Mobile-friendly Interface | Many applicants are mobile-first users who still want a digitally native application. | The Emmy interface is entirely usable from a mobile device | More applicants are able to complete their applications in minutes instead of hours. |
| Immediate feedback | With traditional systems, applicants upload data and wait to hear back if it was accepted, if it was valid etc. | Immediate feedback to users that verification information has been submitted. | Fewer cases requiring caseworker attention and better engagement from applicants. |
| Applicant agency | Existing income verification data sources do not allow the applicant any ability to review the income and provide any helpful information that may help the caseworker approve the application. | Emmy is a consent-based process, with applicants clearly seeing what data will be submitted to state agencies. Applicants can add information that may help the caseworkers approve the case. | Better user perception and concomitant participation. |
| Better access to benefits | Incorrect or missing income data can have significant impacts on benefits. | Emmy directly accesses the client's payroll provider data, connecting to the originating pay data source. | Better access to benefits for eligible applicants. |

### Key Benefits for States

  

|  |  |  |  |
| :-- | :-- | :-- | :-- |
|  | Problem it solves | Emmy feature | Result |
| Data accuracy | Applicant-submitted paper or .pdf records can be incomplete, hard to read, or out of date | Data is imported directly from payroll provider | Accessing data from the payroll provider increases the freshness and accuracy of income data. |
| Cost per application | Existing profiling and income check services have a high cost per application. | Emmy’s costs per transaction are favorable compared to existing commercial sources of income. Further, more accurate data in a standard format reduces the total labor of each application. | Lower costs as programs expand. |
| Fewer caseworker touch points | Paper-based or CSI-based income verification processes have a number of failure points that result in additional case worker interactions. | While CBV doesn't eliminate all errors, it helps to eliminate many common failure points, such as having to contact an applicant over blurry or incomplete document uploads. | Lower caseworker workload with more successful applications the first time. |
| Better applicant engagement | Some applicants aren’t motivated to submit complete data due to mistrust or an overly complex process. | Due to benefits listed in the table above (immediate feedback, applicant agency, mobile-friendly interface) applicants experience an easier and more transparent process | The more Emmy can motivated visitors to complete the application process, the lighter the burden of promotion and communication for states to implement income verification. |

  
  

## HR1 and Emmy

In July 2025, HR1 was signed into law. This statute [adds a "Community Engagement" requirement (CER) for some Medicaid applicants and enrollees](https://www.medicaid.gov/resources-for-states/working-families-tax-cut-legislation/community-engagement). This guidance has a few specific requirements that increase the complexity of the application and renewal processes:

* States can determine the number of previous months, from 1 to 3, where an applicant must demonstrate community engagement.
* When *applying* for Medicaid, states must check if the client met the requirements in at least the prior month. They can verify up to the past 3 months.
* When *renewing* Medicaid, states must check at least the prior month. They can check multiple months, and the months do not need to be consecutive.
* Community engagement can be any combination of work, volunteering, or educational hours.

The in-progress Emmy project has taken on the requirements to support verification of volunteer and education hours, and presenting an easy-to-understand interface showing the applicant their progress in demonstrating community engagement.

These features are under active development by the Emmy team and a first version of these features is projected to be released by the end of Q1 2026.

## How it works

*If you’re a developer excited to get started with Emmy today,* [*check out our implementation guides in our repository*](https://github.com/DSACMS/iv-cbv-payroll)*. If you’re a decision maker who wants to understand how it works at a high level, read on!*

Emmy is hosted on the CMS cloud, providing both a front-end interface and a backend service to handle requests. This service relies on tools like Argyle to verify income with payroll providers. Those tools are hosted on the CMS Cloud.


{% image_with_class "assets/resources/emmy-UI-diagram.png" "diagram of the EMMY service" %}

At the end of a successful integration, applicants will see clear feedback on the status of their verification process, and understand what information is being submitted as part of their application.

## How to adopt Emmy

Ready to get started adopting Emmy for income and community engagement verification? Start by getting in touch with [the Emmy team at CMS.](mailto:emmy@cms.hhs.gov).

If you’d like to see every step of the process, check our [state implementation guide](adoption-checklist/).

