---
title: Foundation | Consent
keywords: foundations, fhir
tags: [foundation,use_case,fhir,rest,api,noccprofile]
sidebar: accessrecord_rest_sidebar
permalink: api_foundation_consent.html
summary: A record of a healthcare consumer’s policy choices, which permits or denies identified recipient(s) or recipient role(s) to perform one or more actions within a given policy context, for specific purposes and periods of time.
---

{% include custom/search.warnbanner.html %}


{% include custom/fhir.reference.html resource="" page="" fhirname="ValueSet" fhirlink="valueset.html" content="-" userlink="-" %}


## 1. Read ##

<div markdown="span" class="alert alert-success" role="alert">
GET [baseUrl]/ValueSet/[id]</div>

{% include custom/read.response.html resource="Consent" content="" %}

## 2. Example ##

{% include custom/search.warn_ri_banner.html %}

### 2.1 Request Query ###

Return the ValueSet for Care Connect Administrative Gender. Replace 'baseUrl' with the actual base Url of the FHIR Server.

#### 2.1.1. cURL ####

{% include custom/embedcurl.html title="Read Care Connect Administrative Gender ValueSet" command="curl -H 'Accept: application/xml+fhir' -H 'Authorization: BEARER [token]' -X GET  '[baseUrl]/ValueSet/CareConnect-AdministrativeGender-1'" %}

### 2.2 Response Body ###

```xml
<ValueSet xmlns="http://hl7.org/fhir">
	<id value="CareConnect-AdministrativeGender-1"/>
	<extension url="http://hl7.org/fhir/StructureDefinition/valueset-map">
		<valueReference>
			<reference value="https://fhir.hl7.org.uk/STU3/ConceptMap/AdministrativeGender-1"/>
		</valueReference>
	</extension>
	<extension url="http://hl7.org/fhir/StructureDefinition/valueset-sourceReference">
		<valueUri value="http://hl7.org/fhir/ValueSet/administrative-gender"/>
	</extension>
	<extension url="http://hl7.org/fhir/StructureDefinition/structuredefinition-wg">
		<valueCode value="pc"/>
	</extension>
	<extension url="http://hl7.org/fhir/StructureDefinition/structuredefinition-fmm">
		<valueInteger value="5"/>
	</extension>
	<extension url="http://hl7.org/fhir/StructureDefinition/structuredefinition-ballot-status">
		<valueString value="Informative"/>
	</extension>
	<url value="https://fhir.hl7.org.uk/STU3/ValueSet/CareConnect-AdministrativeGender-1"/>
	<identifier>
		<system value="urn:ietf:rfc:3986"/>
		<value value="urn:oid:2.16.840.1.113883.4.642.3.1"/>
	</identifier>
	<version value="3.0.1"/>
	<name value="Administrative Gender"/>
	<status value="active"/>
	<date value="2017-04-19T07:46:00+10:00"/>
	<publisher value="HL7 (FHIR Project)"/>
	<contact>
		<telecom>
			<system value="url"/>
			<value value="http://hl7.org/fhir"/>
		</telecom>
		<telecom>
			<system value="email"/>
			<value value="fhir@lists.hl7.org"/>
		</telecom>
	</contact>
	<description value="The gender of a person used for administrative purposes."/>
	<copyright value="Copyright © HL7.org 2011+"/>
	<compose>
		<include>
			<system value="http://hl7.org/fhir/administrative-gender"/>
			<concept>
				<code value="male"/>
				<display value="Male"/>
			</concept>
			<concept>
				<code value="female"/>
				<display value="Female"/>
			</concept>
			<concept>
				<code value="other"/>
				<display value="Other"/>
			</concept>
			<concept>
				<code value="unknown"/>
				<display value="Unknown"/>
			</concept>
		</include>
	</compose>
</ValueSet>
```
