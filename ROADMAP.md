# Roadmap

## Purpose

This roadmap describes the intended development path for the DevPass® Integration Reference repository.

It applies only to public reference and integration work.

It does not commit CREDA Systems to publish proprietary DevPass® identity-binding methods, verification logic, anti-fraud controls, scoring systems, biometric processes, clearance workflows, or other separately maintained technology.

## Current Stage

**Stage 0 — Public Integration Surface**

Current work includes:

* repository governance and licensing;
* public DevPass® architecture;
* verification-result documentation;
* attestation modeling;
* public/private integration boundaries; and
* preparation for limited schemas and examples.

This stage is focused on making DevPass® technically understandable without exposing the proprietary decisioning layer.

## Stage 1 — Reference Schemas

Planned public interfaces may include:

* developer-record schema;
* attestation schema;
* verification-result schema;
* versioning conventions;
* identifier conventions;
* fictional example payloads; and
* validation guidance.

## Stage 2 — Validation and Developer Tooling

Future public work may include:

* schema validation utilities;
* sample verification requests;
* synthetic test fixtures;
* developer integration examples;
* reference client tooling; and
* reproducible example flows.

No capability should be represented as implemented until corresponding public code or documentation exists.

## Stage 3 — External Integrations

Subject to technical review, partnerships, customer needs, and funding, DevPass® may develop public reference integrations for environments such as:

* employer systems;
* recruiting platforms;
* educational institutions;
* credential providers;
* developer platforms;
* workforce marketplaces;
* identity systems; and
* distributed networks.

## Stage 4 — Portable Verification Interfaces

Future public work may include:

* verification APIs;
* SDKs;
* credential and attestation exchange tooling;
* developer-record portability examples;
* integration test harnesses; and
* machine-readable verification receipts.

Publication of integration tooling does not imply publication of the proprietary DevPass® verification engine.

## Repository Principles

Development of this repository should follow several principles:

* expose interfaces, not proprietary decisioning;
* use fictional or synthetic example data only;
* minimize collection and disclosure of identity-related information;
* do not publish placeholder code that implies unsupported capability;
* maintain clear separation between DevPass®, CREDA®, and VTI Foundation Inc.;
* preserve intellectual-property boundaries;
* validate examples before publication;
* distinguish implemented capability from planned work; and
* keep the public repository intentionally small and technically credible.

## Versioning

Early releases may use pre-1.0 semantic versioning, for example:

`v0.1.0-reference`

A `v1.0.0` designation should be reserved for a stable public integration surface with defined interfaces, documentation, examples, and validation behavior.

## Scope Changes

This roadmap may evolve based on:

* implementation experience;
* customer or partner requirements;
* ecosystem integrations;
* grant-funded work;
* privacy and security review;
* intellectual-property review; and
* product-development priorities.

Roadmap items are directional and are not guarantees of delivery.

## Related Notice

See `NOTICE.md` for intellectual-property, trademark, privacy, and platform-boundary information.
