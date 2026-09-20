# DevPass® Attestation Model

## Purpose

This document describes the public reference model for third-party attestations associated with DevPass® developer records.

It is intentionally limited and non-normative.

It does not define the complete DevPass® attestation system, trust model, weighting logic, verifier approval process, fraud controls, or other proprietary implementation methods.

## Attestation Role

An attestation is a structured statement from an external source about a developer, credential, activity, authorship claim, employment relationship, educational achievement, or other relevant fact.

Attestations may contribute evidence to a DevPass® record without requiring the underlying verifier or external system to expose its internal processes.

## Reference Flow

Attestation Source
       │
       ▼
Structured Attestation
       │
       ▼
DevPass® Record
       │
       ▼
Verification Boundary
       │
       ▼
Verification Result

## Potential Attestation Sources

Attestations may originate from sources such as:

* employers;
* educational institutions;
* credential issuers;
* training providers;
* approved reviewers;
* developer platforms;
* project maintainers;
* professional organizations; and
* other implementation-defined sources.

The presence of an attestation does not imply that every attestation source is treated equally.

## Public Attestation Fields

A public reference attestation may include:

* a unique attestation identifier;
* the subject or developer reference;
* the attestation type;
* the issuing source;
* a statement or claim reference;
* issue and expiration timestamps;
* evidence references;
* provenance or integrity references; and
* implementation-specific metadata.

The public schema is intended to represent the attestation interface, not the complete trust model behind it.

## Attestation Types

Illustrative attestation categories may include:

* employment;
* education;
* credential;
* authorship;
* project participation;
* skill evidence;
* reviewer verification; and
* other implementation-defined categories.

This vocabulary is non-normative and may evolve.

## Trust and Weighting

A DevPass® implementation may evaluate factors such as source identity, provenance, evidence quality, recency, scope, or other conditions when processing an attestation.

This repository does not disclose:

* source trust weights;
* verifier ranking;
* scoring formulas;
* fraud thresholds;
* evidence weighting;
* internal acceptance criteria; or
* proprietary attestation resolution logic.

## Privacy and Data Minimization

Attestations may contain sensitive professional or identity-related information.

Public examples in this repository must use fictional or synthetic data.

Real employment records, educational records, identity documents, biometric information, or other sensitive personal information should not be published here.

## Revocation and Expiration

An attestation may include expiration, revocation, or status information where appropriate.

A downstream system should not assume that an attestation remains valid indefinitely merely because it was valid when first issued.

The complete production rules governing attestation lifecycle and validity remain outside this public reference model.

## Relationship to Verification

An attestation may contribute evidence to a verification process.

An attestation does not, by itself, define the final verification outcome.

The DevPass® verification boundary remains responsible for producing the machine-readable result exposed to authorized downstream consumers.

## Non-Normative Status

This document is illustrative and non-normative.

It does not define a complete DevPass® attestation system, a certification process, or rights beyond those expressly provided by the repository license.

See `../NOTICE.md` for additional intellectual-property and platform-boundary information.
