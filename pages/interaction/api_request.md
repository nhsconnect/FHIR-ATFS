---
title: Overview | Request API
keywords: design, overview
tags: [overview]
sidebar: foundations_sidebar
permalink: api_request.html
summary: "Describes the API interaction to request the audit data"
---

{% include important.html content="All information provided below is indicative and subject to on-going review." %}

## Search Audits ##

The Audit and Transparency Service will send a request to the Spine to retrieve the audit data. This can be done using a RESTful interaction.

<div markdown="span" class="alert alert-success" role="alert">
GET [baseUrl]/AuditEvent?entity=[Patient Number]&_include=AuditEvent:patient&_format=json</div>


<pre class="highlight"><code><span class="err">GET [baseUrl]/{{include.content}}AuditEvent?entity=112112112112&_include=AuditEvent:patient&_format=json
</span></code>

Returns a `Bundle` of all audit entries for a Patient with an NHS Number of 112112112112</pre>
