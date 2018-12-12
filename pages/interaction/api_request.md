---
title: Overview | Request API
keywords: design, overview
tags: [overview]
sidebar: foundations_sidebar
permalink: api_request.html
summary: "Describes the API interaction to request the audit data"
---

{% include important.html content="All information provided below is indicative and subject to on-going review." %}

The Audit and Transparency service will send a request to the Spine to retrieve the audit data.

The request will be submitted via an operation and it will be defined using the FHIR OperationDefinition resource. This resource will allow you to define the parameters to send to the Spine and also defines the output resource.

The image below illustrates the flow of data to and from the Spine.

<img src="images/atfs/atfs-operation.png">

More information about the OperationDefinition resource can be found [here]().