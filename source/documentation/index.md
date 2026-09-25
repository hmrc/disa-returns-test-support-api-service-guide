---
title: ISA Returns Test Support API service guide
weight: 1
---

# ISA Returns Test Support API service guide

**Version 0.1** issued 30 September 2026

***

## Service overview

The ISA Returns Test Support API is used in the sandbox environment to initiate and test the reconciliation report 
generation. It enables the simulation of the live service behaviour, allowing you to validate your integration and 
application before deploying to the production environment.

The API also provides an override reporting window facility whose start and end dates can be configured in the sandbox 
environment to test the reporting window behaviour during the monthly return submission period.

## Purpose

Use the ISA Returns Test Support API to:

- trigger test reconciliation reports and validate the integration with the ISA Returns API prior to its implementation 
in the production environment
- test reporting period validation by overriding the default monthly submission reporting window (6th to 19th of each 
month)

The sandbox environment enables you to test the complete end-to-end workflow without affecting the production services 
or the actual customer data.


## Features

Primary features of the ISA Returns Test Support API include the following:

- trigger test reconciliation reports independently of the production service
- test reconciliation report processing and data mapping using simulated reports
- validate the reliable processing of asynchronous notifications
- simulate errors to validate the application responses for various scenarios such as:
    - oversubscription
    - trace and match
    - ineligible investment
- validate the error-handling scenarios across the reconciliation report lifecycle such as errors related to monthly 
submission reporting window restrictions and changes to the post-declaration eligibility status
- test the complete reporting workflow in a controlled environment

## Benefits

Primary benefits of the ISA Returns Test Support API include the following:

- identify integration, processing, and data-mapping issues before production
- validate application behaviour safely in a sandbox environment
- make sure asynchronous events, statuses, and errors are handled correctly
- isolate and resolve integration issues before deployment
- build confidence that the reporting integration functions correctly throughout the end to end process

## Intended audience

The ISA Returns Test Support API service guide provides the information required to integrate with, maintain and use the API within the sandbox environment.

It explains how to:

- initiate and test the reconciliation report generation
- simulate live service behaviour in a controlled environment
- validate application behaviour and integration prior to the production deployment

This document is intended for developers, integrators, and technical users who need to understand and use the API.
