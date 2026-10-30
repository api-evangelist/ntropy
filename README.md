# Ntropy

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Ntropy provides a financial data standardization and enrichment API that turns raw bank transactions and bank-statement PDFs into structured, contextual data. Its products cover transaction enrichment (categorization, entity/merchant identification and recurring-payment detection), bank-statement OCR and extraction, account-holder ledgers, entity resolution, personalization rules, and event webhooks. The v3 REST API (base https://api.ntropy.com) uses API-key header auth, cursor pagination, and a credit-based rate model, and is used for underwriting, transaction approval, personal finance, customer retention and accounting. Ntropy is a fintech company backed by QED Investors; it ships an official Python SDK and a first-party MCP server.

**Areas:** Company · Fintech · Transaction Enrichment · Financial Data · Data Enrichment · Bank Statements · Categorization · Underwriting

## Ntropy on APIs.io

Everything profiled for Ntropy is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/ntropy/](https://apis.io/providers/ntropy/)** — or go straight to one of the APIs or properties below.

### APIs (15)

- [Ntropy Account Holder API](https://apis.io/apis/ntropy/ntropy-account-holder-api/) — Ledger operations
- [Ntropy Bank statements API](https://apis.io/apis/ntropy/ntropy-bank-statements-api/) — The bank statements API allows you to view and enrich transactions found in bank statements. Below is a table with the description of each of the statuses…
- [Ntropy Batches API](https://apis.io/apis/ntropy/ntropy-batches-api/) — The batches API from Ntropy — 3 operation(s) for batches.
- [Ntropy Categories API](https://apis.io/apis/ntropy/ntropy-categories-api/) — The categories API from Ntropy — 2 operation(s) for categories.
- [Ntropy Enrichment API](https://apis.io/apis/ntropy/ntropy-enrichment-api/) — Transaction enrichment.
- [Ntropy Entities API](https://apis.io/apis/ntropy/ntropy-entities-api/) — The entities API from Ntropy — 4 operation(s) for entities.
- [Ntropy Labels API](https://apis.io/apis/ntropy/ntropy-labels-api/) — The Labels API from Ntropy — 2 operation(s) for labels.
- [Ntropy Misc API](https://apis.io/apis/ntropy/ntropy-misc-api/) — Miscellaneous endpoint.
- [Ntropy Personalization API](https://apis.io/apis/ntropy/ntropy-personalization-api/) — The personalization API from Ntropy — 6 operation(s) for personalization.
- [Ntropy Recurrence API](https://apis.io/apis/ntropy/ntropy-recurrence-api/) — The recurrence API from Ntropy — 1 operation(s) for recurrence.
- [Ntropy Reporting API](https://apis.io/apis/ntropy/ntropy-reporting-api/) — The Reporting API from Ntropy — 2 operation(s) for reporting.
- [Ntropy Reports API](https://apis.io/apis/ntropy/ntropy-reports-api/) — The reports API from Ntropy — 2 operation(s) for reports.
- [Ntropy Transactions API](https://apis.io/apis/ntropy/ntropy-transactions-api/) — The transactions API from Ntropy — 3 operation(s) for transactions.
- [Ntropy Webhooks API](https://apis.io/apis/ntropy/ntropy-webhooks-api/) — The webhooks API from Ntropy — 2 operation(s) for webhooks.
- [Ntropy Account Holders API](https://apis.io/apis/ntropy/ntropy-account-holders-api/) — The Account Holders API from Ntropy — 2 operation(s) for account holders.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Ntropy Webhooks](https://apis.io/asyncapis/ntropy/ntropy-webhooks-asyncapi/)

#### Event channels (1)

Individual events and webhooks the provider emits.

- [/](https://apis.io/channels/ntropy/webhook/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [ntropy-mcp.yml](https://apis.io/servers/ntropy/ntropy-mcp-yml/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Ntropy Agentic Access](https://apis.io/agentic-access/ntropy/ntropy-agentic-access/)

#### Collections (16)

Postman and Open Collection request collections.

- [API Reference Account Holder API](https://apis.io/collections/ntropy/open-ntropy-account-holder-api/)
- [API Reference Account Holder accountHolders API](https://apis.io/collections/ntropy/open-ntropy-accountholders-api/)
- [API Reference Account Holder Bank statements API](https://apis.io/collections/ntropy/open-ntropy-bank-statements-api/)
- [API Reference Account Holder bankStatements API](https://apis.io/collections/ntropy/open-ntropy-bankstatements-api/)
- [API Reference Account Holder batches API](https://apis.io/collections/ntropy/open-ntropy-batches-api/)
- [API Reference Account Holder categories API](https://apis.io/collections/ntropy/open-ntropy-categories-api/)
- [API Reference Account Holder Enrichment API](https://apis.io/collections/ntropy/open-ntropy-enrichment-api/)
- [API Reference Account Holder entities API](https://apis.io/collections/ntropy/open-ntropy-entities-api/)
- [API Reference Account Holder Labels API](https://apis.io/collections/ntropy/open-ntropy-labels-api/)
- [API Reference Account Holder Misc API](https://apis.io/collections/ntropy/open-ntropy-misc-api/)
- [API Reference Account Holder personalization API](https://apis.io/collections/ntropy/open-ntropy-personalization-api/)
- [API Reference Account Holder recurrence API](https://apis.io/collections/ntropy/open-ntropy-recurrence-api/)
- [API Reference Account Holder Reporting API](https://apis.io/collections/ntropy/open-ntropy-reporting-api/)
- [API Reference Account Holder reports API](https://apis.io/collections/ntropy/open-ntropy-reports-api/)
- [API Reference Account Holder transactions API](https://apis.io/collections/ntropy/open-ntropy-transactions-api/)
- [API Reference Account Holder webhooks API](https://apis.io/collections/ntropy/open-ntropy-webhooks-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Ntropy Api V3 Overlay](https://apis.io/overlays/ntropy/ntropy-api-v3-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Ntropy Authentication](https://apis.io/security/ntropy/ntropy-authentication/)
- [Ntropy Domain Security](https://apis.io/security/ntropy/ntropy-domain-security/)
- [Ntropy Trust Center](https://apis.io/security/ntropy/ntropy-trust-center/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Ntropy Plans Pricing](https://apis.io/plans/ntropy/ntropy-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Ntropy Rate Limits](https://apis.io/rate-limits/ntropy/ntropy-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://ntropy.com/)
- [Documentation](https://docs.ntropy.com/)
- [Getting started](https://docs.ntropy.com/onboarding)
- [API reference](https://docs.ntropy.com/documentation/api)
- [Sign up](https://dashboard.ntropy.com/)
- [Support](https://docs.ntropy.com/support)
- [Blog](https://ntropy.com/blog)
- [Compliance](https://trust.ntropy.com/)
- [Terms of service](https://ntropy.com/terms)
- [Privacy policy](https://ntropy.com/privacy)
- [GitHub](https://github.com/ntropy-network)
- [Status](https://status.ntropy.com/)

## API Evangelist rating

**Kin Score 55.9** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 58.6 |
| Contract governance | 18.2 |
| Operational transparency | 65.8 |
| Developer ergonomics | 70.8 |
| Access clarity | 42.1 |

**Agent readiness 34.7** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | derived (partial credit) |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | yes |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | mostly |

**Regulatory alignment 26.3** — Insurance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/ntropy/](https://apis.io/providers/ntropy/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Ntropy: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/ntropy/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
