---
name: Process a bank statement with Ntropy
description: Submit a bank-statement PDF, verify its details, and retrieve the extracted, enriched transactions.
api: openapi/ntropy-api-v3-openapi-original.json
operations:
  - post-bank-statement-v-3-bank-statements-post
  - get-bank-statement-statement-info-v-3-bank-statements-id-verify-post
  - get-bank-statement-result-v-3-bank-statements-id-results-get
  - get-bank-statement-v-3-bank-statements-id-get
---

# Process a bank statement with Ntropy

Extract and enrich transactions from a bank-statement PDF (v3, base `https://api.ntropy.com`).

## Steps

1. **Submit the PDF** — `POST /v3/bank_statements`
   (`post-bank-statement-v-3-bank-statements-post`). Returns a bank-statement id;
   processing is asynchronous.
2. **Fast verification (optional)** — `POST /v3/bank_statements/{id}/verify`
   (`get-bank-statement-statement-info-v-3-bank-statements-id-verify-post`) to quickly
   extract account holder, institution and first account for UI/verification.
3. **Poll or subscribe** — check status with `GET /v3/bank_statements/{id}`
   (`get-bank-statement-v-3-bank-statements-id-get`), or register a webhook for
   `bank_statements.completed` / `bank_statements.error` (see asyncapi/ntropy-webhooks-asyncapi.yml)
   instead of polling.
4. **Read results** — `GET /v3/bank_statements/{id}/results`
   (`get-bank-statement-result-v-3-bank-statements-id-results-get`) for the extracted,
   enriched transactions.

## Rules

- Auth: `X-API-KEY` header. Large uploads may return `413`; unsupported types `415`.
- Prefer webhooks over polling to stay within rate limits; webhook deliveries are
  at-least-once (dedupe on `event_id`).
- See errors/ntropy-problem-types.yml and conventions/ntropy-conventions.yml.
