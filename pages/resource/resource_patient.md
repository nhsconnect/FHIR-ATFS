---
title: Patient | Audit & Transparency API
keywords: patient
sidebar: accessrecord_rest_sidebar
permalink: atfs_patient.html
summary: Demographics and other administrative information about an individual receiving care or other health-related services.
---

{% include important.html content="This site is under development by NHS Digital, It is advised not to develop against these specifications until a formal announcement has been made." %}

{% include custom/fhir.reference.html resource="Patient" page="CareConnect-Patient-1" fhirname="Patient" fhirlink="patient.html" content="-" userlink="" %}

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
    <td><code class="highlighter-rouge">name</code></td>
    <td><code class="highlighter-rouge">HumanName</code></td>
    <td>The name of the patient</td>
    <td>Patient.name(official)</td>
</tr>
<tr>
    <td><code class="highlighter-rouge">identifier</code></td>
    <td><code class="highlighter-rouge">Identifier</code></td>
    <td>Patient NHS Number</td>
    <td>Parient.identifier(nhsNumber)</td>
</tr>
<tr>
    <td><code class="highlighter-rouge">birthDate</code></td>
    <td><code class="highlighter-rouge">Date</code></td>
    <td>The date of birth for the patient.</td>
    <td>Patient.birthDate</td>
</tr>
<tr>
    <td><code class="highlighter-rouge">birthPlace</code></td>
    <td><code class="highlighter-rouge">Address</code></td>
    <td>The place of birth for the patient.</td>
    <td>Patient.extension.birthPlace</td>
</tr>
<tr>
    <td><code class="highlighter-rouge">address</code></td>
    <td><code class="highlighter-rouge">Address</code></td>
    <td>Patient address</td>
    <td>Patient.address</td>
</tr>
<tr>
    <td><code class="highlighter-rouge">generalPractitioner</code></td>
    <td><code class="highlighter-rouge">Reference <a href="atfs_organization.html">Organization</a></code></td>
    <td>Registered GP</td>
    <td>Patient.generalPractitioner.display<br/>Patient.generalPractitioner.reference</td>
</tr>
<tr>
    <td><code class="highlighter-rouge">nominatedPharmacy</code></td>
    <td><code class="highlighter-rouge">Reference <a href="atfs_organization.html">Organization</a></code></td>
    <td>Nominated Pharmacy</td>
    <td>Patient.nominatedPharmacy.display<br/>Patient.nominatedPharmacy.reference</td>
</tr>
</table>