---
layout: default
title: API | SynBioCAD
---
The SynBioCAD HTTP API can be used to embed visualization of designs encoded using the [Synthetic Biology Open Language (SBOL)](http://sbolstandard.org) into an existing website or application.

The API currently supports rendering to SVG, PNG, and Microsoft&reg; PowerPoint&reg; formats via three endpoints:

* `POST https://api.biocad.io/render/svg`
* `POST https://api.biocad.io/render/png`
* `POST https://api.biocad.io/render/pptx`

For all of these endpoints, the request should:

* Have the `Content-Type` header `application/rdf+xml`
* Have an SBOL RDF/XML file as the request body

The response will:

* Have the `Content-Type` header `image/svg+xml`, `image/png`, or `application/vnd.openxmlformats-officedocument.presentationml.presentation`
* Contain an SVG, PNG, or PPTX file as the response body


