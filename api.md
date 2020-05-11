---
layout: default
title: API | SynBioCAD
---
The SynBioCAD HTTP API can be used to embed visualization of designs encoded using the [Synthetic Biology Open Language (SBOL)](http://sbolstandard.org) into an existing website or application.

The API currently supports rendering to SVG via the following endpoint:

* `POST https://api.biocad.io/render/svg`

The request should:

* Have the `Content-Type` header `application/rdf+xml`
* Have an SBOL RDF/XML file as the request body

A successful response will:

* Have the `Content-Type` header `image/svg+xml`
* Contain an SVG file as the response body


