---
title: Overview | Response API
keywords: design, build, access, security, overview
tags: [overview]
sidebar: foundations_sidebar
permalink: api_response.html
summary: "Describes the response of the audit and transparency API"
---

{% include important.html content="All information provided below is indicative and subject to on-going review." %}

The response API will output the results to support the Audit and Transparency service.

## Field mappings ##

The table below shows the data retrieved with the FHIR resource mappings.

|**Field**|**Location**|**FHIR Resource**|**Element**|
|Surname|PDS|Patient|name.family|
|First name|PDS|Patient|name.given|
|NHS Number|PDS| Patient|identifier(nhsNumber)|
|Date of Birth|PDS|Patient|birthDate|
|Place of Birth|PDS|Patient|birthPlace|
|Address|PDS|Patient|address|
|Postcode|PDS|Patient|address.postalCode|
|Registered GP|PDS|Patient|generalPractitioner|
|GP Practice code|PDS|Organization|generalPractitioner.reference(Organization)|
|Nominated Pharmacy|PDS|Patient|nominatedPharmacy|
|Pharmacy code|PDS|Organization|nominatedPharmacy.reference(Organization)|
|||||
|Organisation Code|ODS|Organization|identifier(odsOrganisationCode)|
|Organisation Name|ODS|Organization|name|
|Organisation Address|ODS|Organization|address|
|Organisation Postcode|ODS|Organization|address.postalCode|
|Organisation Telephone|ODS|Organization|telecom|
|Organisation Status|ODS|Organization|?|
|Organisation Prescribing Setting|ODS|?||
|||||
|Date Time|Spine|AuditEvent|recorded|
|User ID|Spine|AuditEvent|agent.userId|
|User Name|Spine|AuditEvent|agent.name|
|Business Type|Spine|AuditEvent|businessType|
|Service|Spine|AuditEvent|spineService|


## This diagram illustrates how the FHIR resources are associated in the response ##

<img src="images/atfs/atfs-resources.png">
