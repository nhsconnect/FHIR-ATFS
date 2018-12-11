---
title: Overview | Response API
keywords: design, build, access, security, overview
tags: [design, overview]
sidebar: foundations_sidebar
permalink: api_response.html
summary: "Describes the response of the audit and transparency API"
---

{% include important.html content="All information provided below is indicative and subject to on-going review." %}

The response API will outline the results from the Spine that to support the Audit and Transparency service.

The table below shows the type of data retrieved with the possible FHIR resource mappings.

|Field|Location|FHIR Resource|Element|
|Surname|PDS|CareConnect Patient||
|First name|PDS|Patient||
|NHS Number|PDS| Patient||
|Date of Birth|PDS|Patient||
|Place of Birth|PDS|Patient||
|Address|PDS|Patient||
|Postcode|PDS|Patient||
|Registered GP|PDS|Patient||
|GP Practice code|PDS|Organization||
|Nominated Pharmacy|PDS|Patient||
|Pharmacy code|PDS|Organization||
|||||
|Organisation Code|ODS|Organization||
|Organisation Name|ODS|Organization||
|Organisation Address|ODS|Organization||
|Organisation Postcode|ODS|Organization||
|Organisation Telephone|ODS|Organization||
|Organisation Status|ODS|Organization||
|Organisation Prescribing Setting|ODS|?||
|||||
|Date Time|Spine|AuditEvent||
|User ID|Spine|||
|User Name|Spine|AuditEvent||
|Business Type|Spine|||
|Service|Spine|||
