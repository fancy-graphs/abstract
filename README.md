# fancy-graphs

benchmarking of open source frameworks. With context!

## Goal

Benchmarks are hard to read. This issue is mostly stems from underdocumentation
of the provided examples, making it hard to read the numbers in context.

To achieve this, we use a number of application profiles that need to be
implemented to submit a implementation to the testing and describe how the
feature was implemented.

This allows potential user to grade the important tradeoffs: implementation
effort complexity versus speed.

### Descriptions

Descriptions of submissions are important, so submissions should contain:

* Link to the places where a feature is activated
* Document short-comings
* Document standard or homegrown solutions
* Describe approaches to each component

## Profiles

A profile describes what a submission should implement.

### FFA

The standard framework stack as generated, with good descriptions on what it
gives you out of the box. No changes except webserver stack allowed.

### API

API stacks should come with:

* Routing
* JSON encoding/parsing
* Parameter validation
* SSL support
* ETAG support
* Cache-Control
* Authentication
* Keep-Alive

* Database Access

* (Streaming)

### Website

A standard website stack needs:

* Routing
* CSRF protection
* HSTS protection
* SSL support
* HTML/JS/CSS output (asset delivery)
  - authorized assets
* XSS protection (whitelist, blacklist)
* Cookie/Session (signed, encrypted)
* JSON parsing/encoding
* XHR
* Parameter validation
* Authentication

* Database access

## (Bi-Directional)

* Websockets

