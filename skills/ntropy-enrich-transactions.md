---
name: Enrich bank transactions with Ntropy
description: Create an account holder, submit transactions for synchronous enrichment, and read back the enriched categories, entities and recurrence.
api: openapi/ntropy-api-v3-openapi-original.json
operations:
  - create-account-holder-v-3-account-holders-post
  - post-transaction-v-3-transactions-post
  - get-transaction-v-3-transactions-id-get
  - list-transactions-v-3-transactions-get
---

# Enrich bank transactions with Ntropy

Use the Ntropy Transaction API (v3, base URL `https://api.ntropy.com`) to enrich raw
bank transactions. All requests authenticate with an API key in the `X-API-KEY` header.

## Steps

1. **Create an account holder** — `POST /v3/account_holders`
   (`create-account-holder-v-3-account-holders-post`). Account holders group a party's
   transactions into a ledger and improve enrichment (recurrence, personalization).
2. **Enrich a transaction** — `POST /v3/transactions`
   (`post-transaction-v-3-transactions-post`) with the transaction fields and the
   account-holder id. The response returns entities, categories and recurrence signals.
3. **Retrieve a transaction** — `GET /v3/transactions/{id}`
   (`get-transaction-v-3-transactions-id-get`) to read an enriched transaction later.
4. **List transactions** — `GET /v3/transactions`
   (`list-transactions-v-3-transactions-get`) using cursor pagination: pass `limit` and
   `cursor`, and follow `next_cursor` in the response until it is null.

## Rules

- Auth: `X-API-KEY: <key>` on every request.
- Rate limits are credit-based: 1 credit per enriched transaction, up to 50,000 credits
  refilled at 500/s, max 10 concurrent enrichment operations. Handle `429`
  (NtropyRateLimitError) with backoff and `423` (quota exceeded) by topping up.
- Capture `X-Request-ID` from responses for support/debugging.
- See errors/ntropy-problem-types.yml and conventions/ntropy-conventions.yml.
