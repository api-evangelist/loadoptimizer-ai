---
name: loadoptimizer-ai-submit-optimization-job
description: Submit an optimization job after validating the request.
api: openapi/loadoptimizer-ai-openapi.yml
operations:
- validateJob
- createJob
generated: '2026-10-02'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/loadoptimizer-ai-openapi.yml ; every operationId checked against the contract
---

# loadoptimizer-ai-submit-optimization-job

Submit an optimization job after validating the request.

## Steps

1. 1. Validate the job request using `validateJob` with the request body fields shown in the contract.
2. 2. Submit the optimization job using `createJob` with the same request body fields; include the `Idempotency-Key` header for idempotency.

## Rules

- Include the `Idempotency-Key` header on write operations (`createJob`).
