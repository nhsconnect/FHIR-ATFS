---
title: AuditEvent| Audit & Transparency API
keywords: auditevent
sidebar: accessrecord_rest_sidebar
permalink: atfs_auditevent.html
summary: Demographics and other administrative information about an individual receiving care or other health-related services.
---

{% include important.html content="This site is under development by NHS Digital, It is advised not to develop against these specifications until a formal announcement has been made." %}

{% include custom/fhir.referencemin.html resource="[ATFS-AuditEvent-1](https://fhir.nhs.uk/STU3/StructureDefinition/ATFS-AuditEvent-1)" page="" fhirlink="[AuditEvent](https://www.hl7.org/fhir/stu3/auditevent.html)" content="User Stories" userlink="engage_case_studies.html" %}

## FHIR Elements ##

The following FHIR elements have been identified as key to the implementation:

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
    <td><code class="highlighter-rouge">userId</code></td>
    <td><code class="highlighter-rouge">Identifier</code></td>
    <td>Identifier of the user who accessed the record</td>
    <td>AuditEvent.agent.userId</td>
</tr>
<tr>
    <td><code class="highlighter-rouge">name</code></td>
    <td><code class="highlighter-rouge">string</code></td>
    <td>The name of the user who accessed the record</td>
    <td>AuditEvent.agent.name</td>
</tr>
<tr>
    <td><code class="highlighter-rouge">type</code></td>
    <td><code class="highlighter-rouge">Coding</code></td>
    <td>The type of audit record. This will hold the service name.</td>
    <td>AuditEvent.type</td>
</tr>
<tr>
    <td><code class="highlighter-rouge">subtype</code></td>
    <td><code class="highlighter-rouge">Coding</code></td>
    <td>The business message type</td>
    <td>AuditEvent.subtype</td>
</tr>
</table>