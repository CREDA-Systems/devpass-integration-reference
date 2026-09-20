# DevPass® Integrations

## Purpose

This directory defines the public boundary for external DevPass® integrations.

Integrations connect DevPass® records, attestations, or verification results with authorized external systems without exposing proprietary verification, identity-binding, fraud-control, scoring, or clearance technology.

## Integration Role

A public integration may:

* submit a verification request;
* retrieve an authorized verification result;
* reference a developer record;
* exchange attestation references;
* validate public schema fields;
* consume verification status;
* store an authorized result reference;
* initiate an implementation-defined workflow; or
* return an integration receipt.

## Potential Integration Targets

Future integrations may include:

* employer systems;
* recruiting platforms;
* educational institutions;
* credential providers;
* developer platforms;
* workforce marketplaces;
* identity infrastructure;
* enterprise applications;
* blockchain or distributed-ledger systems; and
* other authorized environments.

No integration is represented as implemented until corresponding public code exists.

## Integration Boundary

```text id="wk6en6"
DevPass® Record / Verification Result
                │
                ▼
        External Integration
                │
                ▼
      Authorized Consumer
```

The integration sits outside the proprietary DevPass® verification boundary.

It should preserve the meaning of the result rather than silently reinterpret the underlying verification outcome.

## Data Minimization

Integrations should request and expose only the information required for the authorized purpose.

Where a verification status or reference is sufficient, integrations should avoid transmitting unnecessary identity, credential, employment, education, biometric, or evidence data.

## Public / Private Boundary

Public integrations may expose:

* request and response mappings;
* public verification-result consumption;
* attestation references;
* credential references;
* validation helpers;
* receipts;
* integration tests; and
* developer documentation.

They should not expose proprietary DevPass® platform internals unless expressly approved for public release.

## Relationship to CREDA®

DevPass® may use CREDA® implementation and integration infrastructure.

A public DevPass® integration does not make the proprietary CREDA® runtime part of this repository.

## Future Repositories

Where substantive integration work exists, separate repositories may be created.

Examples could include:

devpass-employer-reference
devpass-education-reference
devpass-recruiting-reference
devpass-developer-platform-reference

Empty repositories should not be created merely to imply implementation readiness.

## Licensing

Each integration repository should clearly identify its applicable license.

Open-source integration code does not change the ownership or licensing status of proprietary DevPass® or CREDA® technology maintained elsewhere.

## Non-Normative Status

This document describes a public integration boundary only.

It does not define DevPass® product requirements, VTI Foundation Inc. standards, certification criteria, or rights beyond those expressly provided by the applicable repository license.

See `../NOTICE.md` for additional intellectual-property, privacy, and platform-boundary information.
