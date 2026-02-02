---
title: EMMY Integration Guide
description: 'Adoption Checklist for EMMY'
permalink: /resources/integration-guide/
layout: layouts/page
section: resources
tags: emmy
eleventyNavigation:
  parent: emmy-resources
  key: emmy-resources-integrationguide
  order: 3
  title: Integration Guide
sidenav: true
sticky_sidenav: true
---

*This guide is for decision makers trying to add eligibility tools to their state applicant process with EMMY. If you're a developer excited to implement EMMY for your state, [check our full GitHub repository](https://github.com/DSACMS/iv-cbv-payroll).*

Integrating Eligibility Made Easy (EMMY) is a process guided by the needs of an individual state agency. Some questions to ask as you work with the EMMY team:

* Which components of EMMY do I want to implement? 
  * Income
  * Work Hours
  * Volunteer Hours
  * Education Hours/status
* Do we want to use the EMMY interface, or build our own?

The EMMY experience for applicants is designed to be modular, letting you implement just the pieces you need.   
⚠️ Note that EMMY is currently in development, and modularity is a planned feature. [Follow new updates in the GitHub repository](https://github.com/DSACMS/iv-cbv-payroll/commits/main/).

## Implementation using the EMMY interface

The complete EMMY application includes an interface for applicants to interactively offer their consent to load and submit employer, school, and volunteer data.

{% image_with_class "assets/resources/emmy-UI.png" "diagram of the EMMY service" %}

Future updates will include progress indicators that show how close the applicant has gotten to submitting complete data.

⚠️ Note that EMMY doesn't and won't approve applications independently, but progress indicators still yet applicants know if, for example, they've submitted work data for each of the last three months before submission.

When using EMMY with the user interface supplied by CMS, the process of an application will look something like this:

{% image_with_class "assets/resources/emmy-UI-diagram.png" "diagram of the EMMY service" %}

1. An applicant visits a state application portal
2. Applicants are directed to the EMMY UI, customized for that state's service
3. The EMMY applicant interface takes applicant information and loads information from multiple outside data sources
4. Applicants can see and approve the data being submitted
5. The EMMY backend service delivers standardized data to the State Agency with the submitted data

If you have questions about how the EMMY interface can be customized for your state agency, and whether in general an EMMY-provided UI meets your state's and your applicants' needs, get in touch with the EMMY team via email.

## Implementation using the EMMY API Service

If you want to implement your own interface, or if you have an existing application process where EMMY will be used only for additional verification, you may want to use EMMY as an API service. The process looks quite similar:

{% image_with_class "assets/resources/emmy-API-diagram.png" "diagram of the EMMY service" %}

The only major change is that your own application portal will do the work of collecting Applicant interface, and offering the applicant feedback about the data they're submitting.

## How to get started

Start integrating EMMY today by checking out our implementation checklist and reaching out to the EMMY team via email.