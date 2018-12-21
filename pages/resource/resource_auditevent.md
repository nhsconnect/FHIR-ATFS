---
title: AuditEvent | Audit & Transparency API
keywords: auditevent
sidebar: accessrecord_rest_sidebar
permalink: atfs_auditevent.html
summary: Demographics and other administrative information about an individual receiving care or other health-related services.
---

{% include important.html content="This site is under development by NHS Digital, It is advised not to develop against these specifications until a formal announcement has been made." %}

{% include custom/fhir.reference.html resource="AuditEvent" page="ATFS-AuditEvent-1" fhirname="AuditEvent" fhirlink="auditevent.html" content="-" userlink="" %}

## FHIR Elements ##

The following FHIR elements have been identified as key to the implementation:

|**Field**|**Location**|**FHIR Resource**|**Element**|
|Date Time|Spine|AuditEvent|recorded|
|User ID|Spine|AuditEvent|agent.userId|
|User Name|Spine|AuditEvent|agent.name|
|Business Type|Spine|AuditEvent|subtype|
|Service|Spine|AuditEvent|type|

<table style="min-width:100%;width:100%">
<tr id="clinical">
    <th style="width:15%;">Element</th>
    <th style="width:15%;">Type</th>
    <th style="width:30%;">Description</th>
    <th style="width:35%;">Path</th>
</tr>
<tr>
    <td><code class="highlighter-rouge">recorded</code></td>
    <td><code class="highlighter-rouge">instant</code></td>
    <td>The date/time the record was accessed</td>
    <td>AuditEvent.recorded</td>
</tr>
<tr>
    <td><code class="highlighter-rouge">agent</code></td>
    <td><code class="highlighter-rouge">Identifier</code></td>
    <td></td>
    <td>AuditEvent.agent.userId</td>
</tr>
<tr>
    <td><code class="highlighter-rouge">recorded</code></td>
    <td><code class="highlighter-rouge">instant</code></td>
    <td>The date/time the record was accessed</td>
    <td>AuditEvent.recorded</td>
</tr>
</table>