---
title: Resources Overview
keywords: getcarerecord, structured, rest, resource
sidebar: foundations_sidebar
permalink: resource_overview.html
summary: "This page provides an overview of the FHIR STU3 Resources that are required to build the required API."
---

{% include important.html content="This site is under development by NHS Digital, It is advised not to develop against these specifications until a formal announcement has been made." %}

## Resource Association ##

<img src="images/atfs/atfs-resources.png">


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