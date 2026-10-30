# Lithic

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

Lithic is a card issuing and issuer-processor API platform for building virtual and physical card programs - authorization, clearing, KYC/KYB account holder onboarding, programmable authorization rules, real-time Auth Stream Access (ASA) decisioning, disputes, digital wallet tokenization, 3DS authentication, ACH payments, ledgered financial accounts, and settlement reporting. Lithic publishes a full OpenAPI 3.1 specification (github.com/lithic-com/lithic-openapi) backing official Node, Python, Go, Java, and Kotlin SDKs, with a sandbox at sandbox.lithic.com that mirrors production functionality.

**Areas:** Fintech · Card Issuing · Payments · Issuer Processor · KYC · Banking as a Service · Embedded Finance

## Lithic on APIs.io

Everything profiled for Lithic is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/lithic-com/](https://apis.io/providers/lithic-com/)** — or go straight to one of the APIs or properties below.

### APIs (31)

- [Lithic Account API](https://apis.io/apis/lithic-com/lithic-com-account-api/) — Top-level program accounts and their spend limits.
- [Lithic Account Holder API](https://apis.io/apis/lithic-com/lithic-com-account-holder-api/) — KYC/KYB onboarding and management of individual and business account holders.
- [Lithic Auth Rules API](https://apis.io/apis/lithic-com/lithic-com-auth-rules-api/) — Programmable v2 authorization rules, versions, drafts, backtests, and evaluation results.
- [Lithic Auth Stream Access (ASA) API](https://apis.io/apis/lithic-com/lithic-com-auth-stream-access-asa-api/) — Real-time HTTP webhook authorization decisioning in the transaction path.
- [Lithic Balance API](https://apis.io/apis/lithic-com/lithic-com-balance-api/) — Available and pending balances for financial accounts.
- [Lithic Book Transfer API](https://apis.io/apis/lithic-com/lithic-com-book-transfer-api/) — Internal ledger transfers between financial accounts.
- [Lithic Card API](https://apis.io/apis/lithic-com/lithic-com-card-api/) — Virtual and physical card issuance, lifecycle, and digital wallet provisioning.
- [Lithic Card Authorizations API](https://apis.io/apis/lithic-com/lithic-com-card-authorizations-api/) — Responses to real-time authorization challenges.
- [Lithic Card Bulk Orders API](https://apis.io/apis/lithic-com/lithic-com-card-bulk-orders-api/) — Bulk physical card ordering.
- [Lithic Chargeback API](https://apis.io/apis/lithic-com/lithic-com-chargeback-api/) — Legacy v1 dispute (chargeback) submission and evidence.
- [Lithic Credit Product API](https://apis.io/apis/lithic-com/lithic-com-credit-product-api/) — Credit product configuration, extended credit, and prime rates.
- [Lithic Event API](https://apis.io/apis/lithic-com/lithic-com-event-api/) — Events API and webhook event subscription management.
- [Lithic External Bank Account API](https://apis.io/apis/lithic-com/lithic-com-external-bank-account-api/) — External bank accounts used for ACH payments, with prenote and micro-deposit verification.
- [Lithic External Payments API](https://apis.io/apis/lithic-com/lithic-com-external-payments-api/) — Recording and reconciling payments that move outside of Lithic-initiated rails.
- [Lithic Financial Account API](https://apis.io/apis/lithic-com/lithic-com-financial-account-api/) — Ledgered financial accounts, credit configuration, and account activity.
- [Lithic Fraud Report API](https://apis.io/apis/lithic-com/lithic-com-fraud-report-api/) — Fraud reporting on card transactions.
- [Lithic Funding Events API](https://apis.io/apis/lithic-com/lithic-com-funding-events-api/) — Card program funding event reporting.
- [Lithic Hold API](https://apis.io/apis/lithic-com/lithic-com-hold-api/) — Holds placed against financial account balances.
- [Lithic Managed Disputes API](https://apis.io/apis/lithic-com/lithic-com-managed-disputes-api/) — v2 managed disputes (read surface for Lithic-managed dispute handling).
- [Lithic Management Operations API](https://apis.io/apis/lithic-com/lithic-com-management-operations-api/) — Manual ledger adjustments and corrections.
- [Lithic Network Program API](https://apis.io/apis/lithic-com/lithic-com-network-program-api/) — Card network program metadata.
- [Lithic Payment API](https://apis.io/apis/lithic-com/lithic-com-payment-api/) — ACH payments between Lithic financial accounts and external bank accounts.
- [Lithic Responder Endpoints API](https://apis.io/apis/lithic-com/lithic-com-responder-endpoints-api/) — Registration of HTTP endpoints that receive Auth Stream Access (ASA) requests.
- [Lithic Settlement Report API](https://apis.io/apis/lithic-com/lithic-com-settlement-report-api/) — Daily settlement detail, summary, and network total reporting.
- [Lithic Statements API](https://apis.io/apis/lithic-com/lithic-com-statements-api/) — Financial account statements, line items, and loan tapes for credit products.
- [Lithic Status API](https://apis.io/apis/lithic-com/lithic-com-status-api/) — API status check.
- [Lithic Tokenization API](https://apis.io/apis/lithic-com/lithic-com-tokenization-api/) — Digital wallet tokenization (Apple Pay / Google Pay / Samsung Pay) lifecycle and decisioning.
- [Lithic Transaction API](https://apis.io/apis/lithic-com/lithic-com-transaction-api/) — Card transaction authorization, clearing, and simulation.
- [Lithic Transaction Monitoring API](https://apis.io/apis/lithic-com/lithic-com-transaction-monitoring-api/) — Fraud/AML case and queue management for flagged transactions.
- [Lithic Transfer Limits API](https://apis.io/apis/lithic-com/lithic-com-transfer-limits-api/) — The Transfer Limits API from Lithic — 1 operation(s) for transfer limits.
- [Lithic 3 DS API](https://apis.io/apis/lithic-com/lithic-com-3-ds-api/) — 3D Secure e-commerce authentication and decisioning.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### GraphQL (1)

GraphQL schemas.

- [Moved to /providers/lithic-com/](https://apis.io/graphqls/lithic-com/lithic-com-graphql/)

#### MCP servers (2)

Model Context Protocol servers that expose the API to agents.

- [lithic-com](https://apis.io/servers/lithic-com/lithic-com/)
- [mcp](https://apis.io/servers/lithic-com/mcp/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Lithic Com Agentic Access](https://apis.io/agentic-access/lithic-com/lithic-com-agentic-access/)

#### JSON Schema (396)

The data models the API reads and writes.

- [Account Financial Account Type](https://apis.io/schemas/lithic-com/lithic-com-account-financial-account-type/)
- [Account Holder Created](https://apis.io/schemas/lithic-com/lithic-com-account-holder-created/)
- [Account Holder Document Updated](https://apis.io/schemas/lithic-com/lithic-com-account-holder-document-updated/)
- [Account Holder](https://apis.io/schemas/lithic-com/lithic-com-account-holder-response/)
- [Account Holder Updated](https://apis.io/schemas/lithic-com/lithic-com-account-holder-updated/)
- [Account Holder Verification](https://apis.io/schemas/lithic-com/lithic-com-account-holder-verification/)
- [Account Standing](https://apis.io/schemas/lithic-com/lithic-com-account-standing/)
- [Account State](https://apis.io/schemas/lithic-com/lithic-com-account-state/)
- [Auth Rule Account Tokens](https://apis.io/schemas/lithic-com/lithic-com-account-tokens/)
- [Searchable Account Type](https://apis.io/schemas/lithic-com/lithic-com-account-type/)
- [Account Type External](https://apis.io/schemas/lithic-com/lithic-com-account-type-external/)
- [AccountConfiguration](https://apis.io/schemas/lithic-com/lithic-com-accountconfiguration/)
- [AccountHolder](https://apis.io/schemas/lithic-com/lithic-com-accountholder/)
- [AccountHolderBusinessResponse](https://apis.io/schemas/lithic-com/lithic-com-accountholderbusinessresponse/)
- [AccountHolderIndividualResponse](https://apis.io/schemas/lithic-com/lithic-com-accountholderindividualresponse/)
- [AccountHolderVerificationApplication](https://apis.io/schemas/lithic-com/lithic-com-accountholderverificationapplication/)
- [AccountSpendLimits](https://apis.io/schemas/lithic-com/lithic-com-accountspendlimits/)
- [ACH Action](https://apis.io/schemas/lithic-com/lithic-com-ach-action/)
- [AchMethodAttributes](https://apis.io/schemas/lithic-com/lithic-com-achmethodattributes/)
- [action_explanation](https://apis.io/schemas/lithic-com/lithic-com-action-explanation/)
- [Address](https://apis.io/schemas/lithic-com/lithic-com-address/)
- [Address Match Result](https://apis.io/schemas/lithic-com/lithic-com-address-match-result/)
- [Address](https://apis.io/schemas/lithic-com/lithic-com-address-patch/)
- [Amount](https://apis.io/schemas/lithic-com/lithic-com-amount/)
- [Amount Due](https://apis.io/schemas/lithic-com/lithic-com-amount-due/)
- …and 371 more published on APIs.io

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Lithic Com Structure](https://apis.io/json-structure/lithic-com/lithic-com-structure/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Lithic Domain Vocabulary](https://apis.io/vocabularies/lithic-com/lithic-com-vocabulary/)

#### Examples (49)

Example requests and responses.

- [Lithic Com Createeventsubscription Example](https://apis.io/examples/lithic-com/lithic-com-createeventsubscription-example/)
- [Lithic Com Createexternalbankaccount Example](https://apis.io/examples/lithic-com/lithic-com-createexternalbankaccount-example/)
- [Lithic Com Deleteaccountholderentity Example](https://apis.io/examples/lithic-com/lithic-com-deleteaccountholderentity-example/)
- [Lithic Com Get V2Auth Rulesresults Example](https://apis.io/examples/lithic-com/lithic-com-get-v2auth-rulesresults-example/)
- [Lithic Com Getaccountholder Example](https://apis.io/examples/lithic-com/lithic-com-getaccountholder-example/)
- [Lithic Com Getaccountholders Example](https://apis.io/examples/lithic-com/lithic-com-getaccountholders-example/)
- [Lithic Com Getaccounts Example](https://apis.io/examples/lithic-com/lithic-com-getaccounts-example/)
- [Lithic Com Getembedcard Example](https://apis.io/examples/lithic-com/lithic-com-getembedcard-example/)
- [Lithic Com Getenhancedtransactiondata Example](https://apis.io/examples/lithic-com/lithic-com-getenhancedtransactiondata-example/)
- [Lithic Com Getevents Example](https://apis.io/examples/lithic-com/lithic-com-getevents-example/)
- [Lithic Com Geteventsubscription Example](https://apis.io/examples/lithic-com/lithic-com-geteventsubscription-example/)
- [Lithic Com Geteventsubscriptions Example](https://apis.io/examples/lithic-com/lithic-com-geteventsubscriptions-example/)
- [Lithic Com Geteventsubscriptionsecret Example](https://apis.io/examples/lithic-com/lithic-com-geteventsubscriptionsecret-example/)
- [Lithic Com Getnetworkprogram Example](https://apis.io/examples/lithic-com/lithic-com-getnetworkprogram-example/)
- [Lithic Com Getsettlementdetails Example](https://apis.io/examples/lithic-com/lithic-com-getsettlementdetails-example/)
- [Lithic Com Gettokenization Example](https://apis.io/examples/lithic-com/lithic-com-gettokenization-example/)
- [Lithic Com Gettokenizations Example](https://apis.io/examples/lithic-com/lithic-com-gettokenizations-example/)
- [Lithic Com Listenhancedtransactiondata Example](https://apis.io/examples/lithic-com/lithic-com-listenhancedtransactiondata-example/)
- [Lithic Com Patchaccountbytoken Example](https://apis.io/examples/lithic-com/lithic-com-patchaccountbytoken-example/)
- [Lithic Com Patchaccountholder Example](https://apis.io/examples/lithic-com/lithic-com-patchaccountholder-example/)
- [Lithic Com Patchcardbulkorder Example](https://apis.io/examples/lithic-com/lithic-com-patchcardbulkorder-example/)
- [Lithic Com Patchcardbytoken Example](https://apis.io/examples/lithic-com/lithic-com-patchcardbytoken-example/)
- [Lithic Com Post V1Three Ds Decisioningsimulateenter Otp Example](https://apis.io/examples/lithic-com/lithic-com-post-v1three-ds-decisioningsimulateenter-otp-example/)
- [Lithic Com Postaccountholderdocuments Example](https://apis.io/examples/lithic-com/lithic-com-postaccountholderdocuments-example/)
- [Lithic Com Postaccountholderentities Example](https://apis.io/examples/lithic-com/lithic-com-postaccountholderentities-example/)
- …and 24 more published on APIs.io

#### Collections (33)

Postman and Open Collection request collections.

- [Lithic Developer API](https://apis.io/collections/lithic-com/open-lithic/)
- [Lithic API](https://apis.io/collections/lithic-com/open-lithic-com/)
- [Lithic 3DS API](https://apis.io/collections/lithic-com/open-lithic-com-3ds-api/)
- [Lithic 3DS Account API](https://apis.io/collections/lithic-com/open-lithic-com-account-api/)
- [Lithic 3DS Account Holder API](https://apis.io/collections/lithic-com/open-lithic-com-account-holder-api/)
- [Lithic 3DS Auth Rules API](https://apis.io/collections/lithic-com/open-lithic-com-auth-rules-api/)
- [Lithic 3DS Auth Stream Access (ASA) API](https://apis.io/collections/lithic-com/open-lithic-com-auth-stream-access-asa-api/)
- [Lithic 3DS Balance API](https://apis.io/collections/lithic-com/open-lithic-com-balance-api/)
- [Lithic 3DS Book Transfer API](https://apis.io/collections/lithic-com/open-lithic-com-book-transfer-api/)
- [Lithic 3DS Card API](https://apis.io/collections/lithic-com/open-lithic-com-card-api/)
- [Lithic 3DS Card Authorizations API](https://apis.io/collections/lithic-com/open-lithic-com-card-authorizations-api/)
- [Lithic 3DS Card Bulk Orders API](https://apis.io/collections/lithic-com/open-lithic-com-card-bulk-orders-api/)
- [Lithic 3DS Chargeback API](https://apis.io/collections/lithic-com/open-lithic-com-chargeback-api/)
- [Lithic 3DS Credit Product API](https://apis.io/collections/lithic-com/open-lithic-com-credit-product-api/)
- [Lithic 3DS Event API](https://apis.io/collections/lithic-com/open-lithic-com-event-api/)
- [Lithic 3DS External Bank Account API](https://apis.io/collections/lithic-com/open-lithic-com-external-bank-account-api/)
- [Lithic 3DS External Payments API](https://apis.io/collections/lithic-com/open-lithic-com-external-payments-api/)
- [Lithic 3DS Financial Account API](https://apis.io/collections/lithic-com/open-lithic-com-financial-account-api/)
- [Lithic 3DS Fraud Report API](https://apis.io/collections/lithic-com/open-lithic-com-fraud-report-api/)
- [Lithic 3DS Funding Events API](https://apis.io/collections/lithic-com/open-lithic-com-funding-events-api/)
- [Lithic 3DS Hold API](https://apis.io/collections/lithic-com/open-lithic-com-hold-api/)
- [Lithic 3DS Managed Disputes API](https://apis.io/collections/lithic-com/open-lithic-com-managed-disputes-api/)
- [Lithic 3DS Management Operations API](https://apis.io/collections/lithic-com/open-lithic-com-management-operations-api/)
- [Lithic 3DS Network Program API](https://apis.io/collections/lithic-com/open-lithic-com-network-program-api/)
- [Lithic 3DS Payment API](https://apis.io/collections/lithic-com/open-lithic-com-payment-api/)
- …and 8 more published on APIs.io

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Lithic — jsonschema rules](https://apis.io/rules/lithic-com/lithic-com-jsonschema-spectral-rules/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Lithic Com Authentication](https://apis.io/security/lithic-com/lithic-com-authentication/)
- [Lithic Com Domain Security](https://apis.io/security/lithic-com/lithic-com-domain-security/)
- [Lithic Com Trust Center](https://apis.io/security/lithic-com/lithic-com-trust-center/)
- [Lithic Com Vulnerability Disclosure](https://apis.io/security/lithic-com/lithic-com-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Lithic Com Plans Pricing](https://apis.io/plans/lithic-com/lithic-com-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Lithic Com Rate Limits](https://apis.io/rate-limits/lithic-com/lithic-com-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Lithic Com Finops](https://apis.io/finops/lithic-com/lithic-com-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.lithic.com)
- [Documentation](https://docs.lithic.com)
- [Getting started](https://docs.lithic.com/docs/Quickstart)
- [Changelog](https://docs.lithic.com/changelog)
- [Blog](https://www.lithic.com/blog)
- [Terms of service](https://lithic.com/legal/terms)
- [Privacy policy](https://lithic.com/privacy-policy)
- [GitHub](https://github.com/lithic-com)
- [Status](https://status.lithic.com)

## API Evangelist rating

**Kin Score 44.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 50.8 |
| Contract governance | 9.8 |
| Operational transparency | 44.7 |
| Developer ergonomics | 33.3 |
| Access clarity | 36.8 |

**Agent readiness 29.8** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | verified |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 27.7** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/lithic-com/](https://apis.io/providers/lithic-com/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Lithic: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/lithic-com/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
