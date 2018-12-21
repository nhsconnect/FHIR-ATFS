---
title: Overview | Response API
keywords: design, build, access, security, overview
tags: [overview]
sidebar: foundations_sidebar
permalink: api_response.html
summary: "Describes the response of the Audit and Transparency API"
---

{% include important.html content="All information provided below is indicative and subject to on-going review." %}

The response will output the results to support the Audit and Transparency service.

## Response ##

The results of the query will be presented and wrapped using the FHIR [Bundle](http://hl7.org/fhir/bundle.html) resource. By default the response will be returned in JSON.

<script src="https://gist.github.com/sufyanpat/0951b88d32ed7cdf2e8b877af13c8848.js"></script>

## Field mappings ##

The table below shows the data retrieved with the FHIR resource mappings.

|**Field**|**Location**|**FHIR Resource**|**Element**|
|Date Time|Spine|AuditEvent|recorded|
|User ID|Spine|AuditEvent|agent.userId|
|User Name|Spine|AuditEvent|agent.name|
|Business Type|Spine|AuditEvent|subtype|
|Service|Spine|AuditEvent|type|
|||||
|Surname|PDS|Patient|name.family|
|First name|PDS|Patient|name.given|
|NHS Number|PDS| Patient|identifier(nhsNumber)|
|Date of Birth|PDS|Patient|birthDate|
|Place of Birth|PDS|Patient|birthPlace|
|Address|PDS|Patient|address|
|Postcode|PDS|Patient|address.postalCode|
|Registered GP|ODS|Organization.reference|ODS API|
|Nominated Pharmacy|PDS|Patient|nominatedPharmacy|
|||||
|Organisation Code|ODS|Organization|ODS API|
|Organisation Name|ODS|Organization|ODS API|
|Organisation Address|ODS|Organization|ODS API|
|Organisation Postcode|ODS|Organization|ODS API|
|Organisation Telephone|ODS|Organization|ODS API|

