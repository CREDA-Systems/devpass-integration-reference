# DevPass® Integration Boundaries

## Purpose

This document defines the public integration boundary between DevPass® and external systems.

It is intended to support interoperability while preserving the separation between public integration interfaces and proprietary DevPass® verification, identity, fraud-control, scoring, and clearance technology.

## Core Boundary

The public reference model separates:

1. developer records and supporting attestations;
2. proprietary verification processing;
3. machine-readable verification results; and
4. external systems that consume those results.

Developer Record / Attestations
            │
            ▼
   Verification Boundary
            │
            ▼
    Verification Result
            │
            ▼
    External Integration

## Public Integration Surface

Public integrations may consume or exchange:

* developer-record references;
* credential references;
* attestation references;
* verification-result identifiers;
* verification status;
* timestamps;
* validity information;
* provenance or integrity references;
* scope information; and
* implementation-specific metadata.

These interfaces are intended to support interoperability without exposing proprietary internal decisioning.

## External Systems

Potential external consumers may include:

* employers;
* recruiters;
* educational institutions;
* developer platforms;
* credential providers;
* workforce marketplaces;
* identity providers;
* enterprise systems; and
* other authorized applications.

## What External Integrations May Do

An external integration may:

* request verification;
* retrieve a permitted verification result;
* reference an attestation or credential;
* validate a public schema;
* consume a status or validity field;
* store an authorized result reference;
* initiate an implementation-defined workflow; or
* return an integration receipt.

## What External Integrations Do Not Automatically Receive

Public integration does not imply access to:

* proprietary scoring logic;
* source trust weights;
* fraud models;
* biometric information;
* identity-binding procedures;
* reviewer weighting;
* live-defense processes;
* clearance logic;
* internal risk signals;
* confidential evidence; or
* production user data.

Access to any non-public information must be separately authorized and governed.

## Data Minimization

External integrations should request and consume only the information needed for the authorized purpose.

A verification result should not expose underlying identity, employment, education, biometric, or credential evidence where a narrower machine-readable result is sufficient.

## Product Decisions and External Decisions

DevPass® may provide a verification result or other machine-readable output.

External employers, schools, recruiters, platforms, or other consumers remain responsible for their own hiring, admissions, credentialing, access, or business decisions.

A DevPass® verification result should not be interpreted as automatically making those downstream decisions.

## Relationship to CREDA®

DevPass® may use CREDA® implementation and integration infrastructure.

A public DevPass® integration may therefore interact with CREDA® services or interfaces without exposing the proprietary CREDA runtime.

The public boundary should preserve the distinction between:

* DevPass® product data and outputs;
* CREDA® implementation infrastructure; and
* external consuming systems.

## Relationship to VTI Foundation Inc.

VTI Foundation Inc. develops and stewards standards, reference architectures, and governance frameworks separately from CREDA Systems.

Public DevPass® integration does not establish VTI Foundation Inc. conformance, certification, verification, endorsement, or accreditation.

## Public / Private Boundary

This repository may expose:

* schemas;
* examples;
* public result formats;
* attestation structures;
* integration guidance;
* developer documentation; and
* approved public integration code.

It does not, by default, expose:

* proprietary identity-binding methods;
* fraud detection;
* scoring;
* biometric workflows;
* reviewer or verifier trust weighting;
* clearance decisioning;
* internal evidence processing;
* anti-gaming mechanisms;
* production security architecture; or
* unpublished patent-sensitive implementation details.

## Non-Normative Status

This document describes a public integration boundary only.

It does not define a complete DevPass® product implementation or create rights beyond those expressly provided by the repository license.

See `../NOTICE.md` for additional intellectual-property and platform-boundary information.
