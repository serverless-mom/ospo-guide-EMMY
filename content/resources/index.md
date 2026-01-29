---
title: Resources
description: 'What is EMMY?'
permalink: /resources/
layout: layouts/page
section: resources
tags: ospo
eleventyNavigation:
  parent: ospo-resources
  key: ospo-resources-main
  order: 1
  title: What is EMMY?
sidenav: true
sticky_sidenav: true
---

# Income Verification (EMMY): A Guide for Leaders

*This guide is intended for leadership teams evaluating EMMY as an option, if you already know what EMMY does and are excited to get started,* [*check out the git repository here*](https://github.com/DSACMS/iv-cbv-payroll)*.* 

## Why EMMY

  

Eligibility Made Easy (EMMY) is a project to allow applicants to verify their income and community engagement directly using payroll providers and educational records. EMMY was developed and is supported by CMS in order to offer states a drop-in component for their application process to allow applicants to apply for state benefits more easily. This is part of a more comprehensive process to [improve data services for benefits delivery](https://assets.performance.gov/cx/files/OMB-CX-LifeExperience-FFS-ImprovingData.pdf).

EMMY uses consent-based verification (CBV) with multiple data sources, making the process much faster and more efficient than a simple document-upload service. CBV enables additional cost avoidance by optimizing manual document review processes. Rather than having to process incorrect or blurry documents, consent-based verification produces an easily consumed report with essential information. Verification information is returned in a standardized format easy for other systems to process (JSON), allowing integration with existing state systems. 

EMMY is under active development by CMS, with new updates released on a weekly cadence. [Check out the release history](https://github.com/DSACMS/iv-cbv-payroll/releases) on the GitHub repository. By participating now, you can help shape the development of EMMY and ensure it meets your states’ requirements.

### Key Benefits for Applicants

  

|  |  |  |  |
| :-- | :-- | :-- | :-- |
|  | Problem it solves | EMMY feature | Result |
| No working with paper paystubs or organizing your PDFs | Showing income has historically been a long and arduous process. | The basic design of EMMY is a massive streamlining of the classic income verification process. | EMMY delivers huge savings of time and effort for every users. |
| Detection of lost jobs | Verifying that a job has ended used to require a phone call to the former employer. | With payroll provider integration, EMMY can detect the loss of a job without special representative attention. | A much easier process for state agencies and applicants. |
| Mobile-friendly Interface | Many applicants are mobile-first users who still want a digitally native application. | The EMMY interface is entirely usable from a mobile device | More applicants are able to complete their applications in minutes instead of hours. |
| Immediate feedback | With traditional systems, applicants upload data and wait to hear back if it was accepted, if it was valid etc. | Immediate feedback to users that verification information has been submitted. | Fewer cases requiring caseworker attention and better engagement from applicants. |
| Applicant agency | Existing income verification data sources do not allow the applicant any ability to review the income and provide any helpful information that may help the caseworker approve the application. | EMMY is a consent-based process, with applicants clearly seeing what data will be submitted to state agencies. Applicants can add information that may help the caseworkers approve the case. | Better user perception and concomitant participation. |
| Better access to benefits | Incorrect or missing income data can have significant impacts on benefits. | EMMY directly accesses the client's payroll provider data, connecting to the originating pay data source. | Better access to benefits for eligible applicants. |

### Key Benefits for States

  

|  |  |  |  |
| :-- | :-- | :-- | :-- |
|  | Problem it solves | EMMY feature | Result |
| Data accuracy | Applicant-submitted paper or .pdf records can be incomplete, hard to read, or out of date | Data is imported directly from payroll provider | Accessing data from the payroll provider increases the freshness and accuracy of income data. |
| Cost per application | Existing profiling and income check services have a high cost per application. | EMMY’s costs per transaction are favorable compared to existing commercial sources of income. | Lower costs as programs expand. |
| Fewer caseworker touch points | Paper-based or CSI-based income verification processes have a number of failure points that result in additional case worker interactions. | While CBV doesn't eliminate all errors, it helps to eliminate many common failure points, such as having to contact an applicant over blurry or incomplete document uploads. | Lower caseworker workload with more successful applications the first time. |
| Better applicant engagement | Some applicants aren’t motivated to submit complete data due to mistrust or an overly complex process. | Due to benefits listed in the table above (immediate feedback, applicant agency, mobile-friendly interface) applicants experience an easier and more transparent process | The more EMMY can motivated visitors to complete the application process, the lighter the burden of promotion and communication for states to implement income verification. |

  
  

## HR1 and EMMY

In July 2025, HR1 was signed into law. This statute [adds a "Community Engagement" requirement (CER) for some Medicaid applicants and enrollees](https://www.medicaid.gov/resources-for-states/working-families-tax-cut-legislation/community-engagement). This guidance has a few specific requirements that increase the complexity of the application and renewal processes:

* States can determine the number of previous months, from 1 to 3, where an applicant must demonstrate community engagement.
* When *applying* for Medicaid, states must check if the client met the requirements in at least the prior month. They can verify up to the past 3 months.
* When *renewing* Medicaid, states must check at least the prior month. They can check multiple months, and the months do not need to be consecutive.
* Community engagement can be any combination of work, volunteering, or educational hours.

Along with verifying income, the in-progress EMMY project has taken on the requirements to support verification of volunteer and education hours, and presenting an easy-to-understand interface showing the applicant their progress in demonstrating community engagement.

These features are under active development by the EMMY team and a first version of these features is projected to be released by the end of Q1 2026.

## How it works

*If you’re a developer excited to get started with EMMY today,* [*check out our implementation guides in our repository*](https://github.com/DSACMS/iv-cbv-payroll)*. If you’re a decision maker who wants to understand how it works at a high level, read on!*

EMMY is hosted on the CMS cloud, providing both a front-end interface and a backend service to handle requests. This service relies on tools like Argyle to verify income with payroll providers. Those tools are hosted on the CMS Cloud.


At the end of a successful integration, applicants will see clear feedback on the status of their verification process, and understand what information is being submitted as part of their application.

## How to adopt EMMY

Ready to get started adopting EMMY for income and community engagement verification? Start by getting in touch [with the EMMY team](mailto:emmy@cms.hhs.gov).

If you’d like to see every step of the process, check our state implementation guide.