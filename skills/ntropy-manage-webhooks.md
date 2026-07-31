---
name: Manage Ntropy webhooks
description: Register a webhook for asynchronous events, verify deliveries with the token header, and re-enable a disabled webhook.
api: openapi/ntropy-api-v3-openapi-original.json
operations:
  - post-webhook-v-3-webhooks-post
  - get-webhooks-v-3-webhooks-get
  - get-webhook-v-3-webhooks-id-get
  - patch-webhook-v-3-webhooks-id-patch
  - delete-webhook-v-3-webhooks-id-delete
---

# Manage Ntropy webhooks

Receive real-time events instead of polling (v3, base `https://api.ntropy.com`).

## Steps

1. **Create a webhook** — `POST /v3/webhooks`
   (`post-webhook-v-3-webhooks-post`) with a `url` and the `events` to subscribe to
   (e.g. `batches.completed`, `bank_statements.completed`, `reports.resolved`). Set an
   optional `token`; it is returned in the `X-Ntropy-Token` header on each delivery.
   Limit: 10 webhooks per organization.
2. **List / read** — `GET /v3/webhooks` (`get-webhooks-v-3-webhooks-get`) and
   `GET /v3/webhooks/{id}` (`get-webhook-v-3-webhooks-id-get`).
3. **Re-enable a disabled webhook** — `PATCH /v3/webhooks/{id}`
   (`patch-webhook-v-3-webhooks-id-patch`) with `enabled: true`. Ntropy disables webhooks
   after too many consecutive non-2xx responses.
4. **Delete** — `DELETE /v3/webhooks/{id}` (`delete-webhook-v-3-webhooks-id-delete`).

## Rules

- Respond `2xx` within 10 seconds; defer heavy work. Non-2xx/timeouts are retried with
  the same `event_id` for up to 24h. Deliveries are at-least-once — dedupe on `event_id`.
- Validate `X-Ntropy-Token` if you set one. Event body: `{ event_id, event_type, data }`.
- Event catalog and schema: asyncapi/ntropy-webhooks-asyncapi.yml.
