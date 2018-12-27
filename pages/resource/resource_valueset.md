---
title: ValueSet | Audit & Transparency API
keywords: foundations, fhir
tags: [foundation,use_case,fhir,rest,api,noccprofile]
sidebar: overview_sidebar
permalink: atfs_valueset.html
summary: A ValueSet selects a set of codes from those defined by one or more code systems.
---

{% include custom/search.warnbanner.html %}

{% include custom/fhir.referencemin.html resource="[ATFS Business Message Type](https://directory.spineservices.nhs.uk/STU3/ValueSet/ATFS-BusinessMessageType-1)" resource1="[ATFS Service](https://fhir.nhs.uk/STU3/ValueSet/ATFS-AuditService-1)" page="" fhirlink="[ValueSet](http://www.hl7.org/fhir/stu3/valueset.html)" content="User Stories" userlink="" %}


## 1. Read ##

<div markdown="span" class="alert alert-success" role="alert">
GET [baseUrl]/ValueSet/[id]</div>

{% include custom/read.response.html resource="ValueSet" content="" %}

## 2. Example ##

### 2.1 Request Query ###

Return the ValueSet lookup API 'ATFS Audit Service'. Replace 'baseUrl' with the actual base Url of the FHIR Server.

<div markdown="span" class="alert alert-success" role="alert">
GET https://fhir.nhs.uk/STU3/CodeSystem/ATFS-AuditService-1</div>

{% include custom/search.response.headers.html resource="ValueSet"  %}

### 2.3 Response Body ###

<script src="https://gist.github.com/IOPS-DEV/b28db7655f3a4fdf921f249bedc316cc.js"></script>
