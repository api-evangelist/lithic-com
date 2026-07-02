# Lithic (lithic-com)

Lithic is a card issuing and issuer-processor API platform for building virtual and physical card programs - authorization, clearing, KYC/KYB account holder onboarding, programmable authorization rules, real-time Auth Stream Access (ASA) decisioning, disputes, digital wallet tokenization, 3DS authentication, ACH payments, ledgered financial accounts, and settlement reporting. Lithic publishes a full OpenAPI 3.1 specification ([github.com/lithic-com/lithic-openapi](https://github.com/lithic-com/lithic-openapi)) backing official Node, Python, Go, Java, and Kotlin SDKs, with a sandbox at `sandbox.lithic.com` that mirrors production functionality.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/apis.yml)

## Tags

- Fintech
- Card Issuing
- Payments
- Issuer Processor
- KYC
- Banking as a Service

## Timestamps

- **Created:** 2026-07-02
- **Modified:** 2026-07-02

## APIs

### Lithic Account Holders API

Create and manage individual (KYC) and business (KYB) account holders - identity verification workflows (KYC_BASIC, KYC_BYO, KYC_EXEMPT, KYB_BASIC), document upload for remediation, and beneficial owner / control person management.

- **Human URL:** [https://docs.lithic.com/docs/account-holders-kyc](https://docs.lithic.com/docs/account-holders-kyc)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/account-holders-kyc)
- [Documentation](https://docs.lithic.com/docs/account-holders-kyb)
- [API Reference](https://docs.lithic.com/reference/getaccountholders)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Accounts API

List and retrieve accounts (created 1:1 with an account holder), update daily/monthly/lifetime spend limits, and fetch an account's available spend limits and fraud/velocity signals.

- **Human URL:** [https://docs.lithic.com/docs/spend-limits](https://docs.lithic.com/docs/spend-limits)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/spend-limits)
- [API Reference](https://docs.lithic.com/reference/getaccounts)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Cards API

Issue and manage virtual and physical cards - create, update, reissue, renew, and convert virtual cards to physical; card programs, digital card art, bulk card orders, card balances and financial transactions, the embedded card UI, and Apple Pay / Google Pay push provisioning.

- **Human URL:** [https://docs.lithic.com/docs/cards](https://docs.lithic.com/docs/cards)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/cards)
- [Documentation](https://docs.lithic.com/docs/managing-cards)
- [Documentation](https://docs.lithic.com/docs/physical-cards-setup-guide)
- [API Reference](https://docs.lithic.com/reference/postcards)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Transactions & Authorizations API

List and retrieve card transactions, respond to authorization challenges, expire authorizations, route transactions, pull enhanced commercial (Level II/III) data, and fully simulate the authorization -> clearing -> void/return lifecycle in Sandbox.

- **Human URL:** [https://docs.lithic.com/docs/transaction-flow](https://docs.lithic.com/docs/transaction-flow)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/transaction-flow)
- [Documentation](https://docs.lithic.com/docs/transactions)
- [Documentation](https://docs.lithic.com/docs/simulating-transactions)
- [API Reference](https://docs.lithic.com/reference/postsimulateauthorize)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Authorization Rules API

Create, draft, promote, and backtest v2 programmable authorization rules (velocity limits, MCC/country/risk-score conditions) scoped to a card, account, or program, including calculated feature values and rule evaluation result history.

- **Human URL:** [https://docs.lithic.com/docs/authorization-rules-v2](https://docs.lithic.com/docs/authorization-rules-v2)
- **Base URL:** `https://api.lithic.com/v2`

#### Properties

- [Documentation](https://docs.lithic.com/docs/authorization-rules-v2)
- [Documentation](https://docs.lithic.com/docs/about-authorization-intelligence)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Real-Time Decisioning API

Register and manage the HTTP responder endpoint that receives Auth Stream Access (ASA) requests synchronously inside the authorization path (APPROVED/CHALLENGE/decline within a 6-second window), plus the equivalent 3DS Decisioning webhook for step-up challenge decisions, and HMAC secret retrieval/rotation for both.

- **Human URL:** [https://docs.lithic.com/docs/auth-stream-access-asa](https://docs.lithic.com/docs/auth-stream-access-asa)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/auth-stream-access-asa)
- [Documentation](https://docs.lithic.com/docs/about-3ds)
- [Documentation](https://docs.lithic.com/docs/3ds-decisioning)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Disputes API

Submit and withdraw chargeback requests on settled transactions, upload and manage evidence, and read v2 managed disputes for programs where Lithic handles dispute processing on the issuer's behalf. Lithic documents the Disputes API as an Enterprise product.

- **Human URL:** [https://docs.lithic.com/docs/disputes-api](https://docs.lithic.com/docs/disputes-api)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/disputes-api)
- [Documentation](https://docs.lithic.com/docs/tracking-disputes)
- [API Reference](https://docs.lithic.com/reference/postdisputes)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Events & Webhooks API

Manage event subscriptions (register a webhook URL, rotate its signing secret, resend or replay-missing messages after downtime), list and retrieve individual events and their delivery attempts, and simulate any of the 60+ documented event types in Sandbox.

- **Human URL:** [https://docs.lithic.com/docs/events-api](https://docs.lithic.com/docs/events-api)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/events-api)
- [Documentation](https://docs.lithic.com/docs/simulating-webhooks)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Financial Accounts & Statements API

Create and manage ISSUING, OPERATING, RESERVE, and CHARGE_CARD financial accounts, register account numbers, configure credit limits and interest tier schedules, list account activity and financial transactions, and retrieve statements, statement line items, and loan tapes.

- **Human URL:** [https://docs.lithic.com/docs/financial-accounts](https://docs.lithic.com/docs/financial-accounts)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/financial-accounts)
- [Documentation](https://docs.lithic.com/docs/ledger-overview)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Balances & Holds API

Read available and pending balances across all or a specific financial account, and create, retrieve, or void holds placed against a financial account's balance.

- **Human URL:** [https://docs.lithic.com/docs/ledger-overview](https://docs.lithic.com/docs/ledger-overview)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/ledger-overview)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Payments (ACH) API

Move funds via ACH between a Lithic financial account and a verified external bank account - create, retry, and return payments - with Sandbox simulation of receipt, release, and return events across the ACH lifecycle.

- **Human URL:** [https://docs.lithic.com/docs/payments-api](https://docs.lithic.com/docs/payments-api)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/payments-api)
- [Documentation](https://docs.lithic.com/docs/ach-overview)
- [Documentation](https://docs.lithic.com/docs/ach-payments-lifecycle)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Ledger, Transfers & Settlement API

Move money internally between financial accounts with book transfers, post and reverse manual management operations (ledger corrections), enforce transfer limits, look up card network programs, and reconcile daily cash movement with settlement detail/summary reports, network totals, and per-program funding events. Lithic documents Settlement as an Enterprise, production-only product.

- **Human URL:** [https://docs.lithic.com/docs/book-transfers](https://docs.lithic.com/docs/book-transfers)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/book-transfers)
- [Documentation](https://docs.lithic.com/docs/settlement-reporting)
- [API Reference](https://docs.lithic.com/reference/getsettlementdetails)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic External Payments & Bank Accounts API

Add and verify external bank accounts via prenote or micro-deposits, pause/unpause and retry verification, and create and manage external payments - settle, release, cancel, or reverse - for funds movement that occurs outside of Lithic-initiated ACH rails.

- **Human URL:** [https://docs.lithic.com/docs/external-accounts-api](https://docs.lithic.com/docs/external-accounts-api)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/external-accounts-api)
- [Documentation](https://docs.lithic.com/docs/disbursements)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Tokenization & Digital Wallets API

List and manage a card's digital wallet tokenizations - pause, unpause, activate, deactivate, resend activation codes, and update digital card art - plus the Tokenization Decisioning HMAC secret used to verify the real-time webhook Lithic sends when a cardholder adds a card to Apple Pay, Google Pay, or Samsung Pay.

- **Human URL:** [https://docs.lithic.com/docs/about-digital-wallets](https://docs.lithic.com/docs/about-digital-wallets)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/about-digital-wallets)
- [Documentation](https://docs.lithic.com/docs/push-provisioning)
- [Documentation](https://docs.lithic.com/docs/web-push-provisioning)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lithic Fraud & Transaction Monitoring API

File and retrieve fraud reports on card transactions, and manage transaction monitoring cases and queues - case activity, linked transactions and cards, comments, and file attachments - for AML/fraud review workflows.

- **Human URL:** [https://docs.lithic.com/docs/about-authorization-intelligence](https://docs.lithic.com/docs/about-authorization-intelligence)
- **Base URL:** `https://api.lithic.com/v1`

#### Properties

- [Documentation](https://docs.lithic.com/docs/about-authorization-intelligence)
- [API Reference](https://docs.lithic.com/reference/getfraudreport)
- [OpenAPI](openapi/lithic-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lithic-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lithic-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/lithic-com)
- [LinkedIn](https://www.linkedin.com/company/lithic)
- [Website](https://www.lithic.com)
- [Documentation](https://docs.lithic.com)
- [Plans](plans/lithic-com-plans-pricing.yml)
- [Rate Limits](rate-limits/lithic-com-rate-limits.yml)
- [Fin Ops](finops/lithic-com-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
