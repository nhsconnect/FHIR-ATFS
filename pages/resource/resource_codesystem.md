---
title: CodeSystem | Audit & Transparency API
keywords: foundations, fhir
tags: [foundation,use_case,fhir,rest,api,noccprofile]
sidebar: overview_sidebar
permalink: atfs_codesystem.html
summary: A CodeSystem defines a set of codes with meanings.
---

{% include custom/search.warnbanner.html %}

{% include custom/fhir.referencemin.html resource="[ATFS Business Message Type](https://directory.spineservices.nhs.uk/STU3/CodeSystem/ATFS-BusinessMessageType-1)" resource1="[ATFS Service](https://fhir.nhs.uk/STU3/CodeSystem/ATFS-AuditService-1)" page="" fhirlink="[CodeSystem](http://www.hl7.org/fhir/stu3/codesystem.html)" content="User Stories" userlink="" %}


## 1. Read ##

<div markdown="span" class="alert alert-success" role="alert">
GET [baseUrl]/CodeSystem/[id]</div>

{% include custom/read.response.html resource="CodeSystem" content="" %}

## 2. Example ##

### 2.1 Request Query ###

Return the CodeSystem ATFS lookup API 'ATFS Business Message Type'. Replace 'baseUrl' with the actual base Url of the FHIR Server.

<div markdown="span" class="alert alert-success" role="alert">
GET https://fhir.nhs.uk/STU3/CodeSystem/ATFS-BusinessMessageType-1</div>

{% include custom/search.response.headers.html resource="CodeSystem"  %}


### 2.3 Response Body ###

<script src="https://gist.github.com/IOPS-DEV/dd835e309db1b643f056e39d02c886ce.js"></script>
