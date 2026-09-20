# Reference Schemas

## Purpose

The schemas in this directory define a limited, non-normative public integration surface for DevPass®.

They are intended to support interoperability, developer integration, credential portability, technical evaluation, and future public reference work.

They do not define the complete DevPass® platform, proprietary verification methods, identity-binding processes, fraud controls, scoring systems, biometric workflows, clearance logic, or VTI Foundation Inc. standards.

## Current Schemas

### `developer-record.schema.json`

Provides a minimal public representation of a DevPass® developer record.

### `attestation.schema.json`

Provides a minimal public representation of a third-party attestation associated with a developer record.

### `verification-result.schema.json`

Provides a minimal public representation of a machine-readable DevPass® verification result.

## Non-Normative Status

These schemas are public integration interfaces only.

They do not:

* define the complete DevPass® implementation;
* expose proprietary verification or decisioning logic;
* define Trust-State® conformance;
* establish certification requirements;
* replace any official VTI Foundation Inc. specification; or
* grant rights beyond those provided by the repository license.

## Versioning

Early schemas may use pre-1.0 interface versions such as:

`0.1`

A schema version identifies the version of the public interface only.

It should not be interpreted as a version number for the DevPass® platform, CREDA®, any VTI Foundation Inc. standard, or any certification program.

## Privacy and Example Data

Schemas may represent identity, credential, employment, education, authorship, or attestation-related information.

Public examples must use fictional or synthetic data only.

Real production personal information, biometric data, credential evidence, or confidential records should not be published in this repository.

## Extension Guidance

Implementations may require additional fields.

Extensions should avoid changing the meaning of defined public fields and should not imply DevPass® endorsement, VTI Foundation Inc. conformance, or certification merely because they are structurally compatible with these schemas.

## Intellectual Property

See `../NOTICE.md` for additional information concerning proprietary DevPass® technology, CREDA® technology, standards, trademarks, patents, privacy, and pre-existing intellectual property.
