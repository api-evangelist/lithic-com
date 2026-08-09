# Lithic GraphQL Schema

## Overview

This document describes a conceptual GraphQL schema for the Lithic card-issuing and program-management platform. Lithic provides a REST API; this schema represents the same domain expressed as GraphQL types, queries, and mutations for integration reference and tooling purposes.

Lithic's platform covers card issuance, account management, transaction processing, authorization rules, financial accounts, ACH/wire payments, KYC/KYB account-holder verification, tokenization, disputes, and webhooks.

- **Source docs**: https://docs.lithic.com/docs/
- **REST API reference**: https://docs.lithic.com/reference
- **GitHub**: https://github.com/lithic-com
- **Schema file**: lithic-schema.graphql

## Domain Model

### Cards

Lithic's core resource is the **Card**. Cards can be virtual, physical, or digital-wallet tokens. Each card belongs to an Account and optionally a CardProgram. Key types:

- `Card` — top-level card resource with token, state, type, spend limits, and memo
- `CardDetails` — sensitive PAN, CVV, expiry (returned only via secure endpoints)
- `CardState` — enum: OPEN, PAUSED, CLOSED, PENDING_FULFILLMENT, PENDING_ACTIVATION
- `CardType` — enum: VIRTUAL, PHYSICAL, MERCHANT_LOCKED, SINGLE_USE
- `VirtualCard`, `PhysicalCard`, `DigitalCard` — specialized card views
- `SpendLimit` / `SpendLimitDuration` — per-card velocity controls

### Accounts

An **Account** is the top-level container for cards and balances. Account holders are verified via KYC (individuals) or KYB (businesses).

- `Account`, `AccountDetails`, `AccountState`
- `AccountBalance` — available, pending, and ledger balances
- `AccountSpendLimit` — aggregate velocity controls at account level
- `Kyc`, `KybInfo`, `Document`, `UserDocument`

### Transactions

Every card swipe, ACH movement, or book transfer produces a **Transaction**. The lifecycle moves through authorization, clearing, and settlement.

- `Transaction`, `TransactionDetails`, `TransactionResult`, `TransactionType`
- `Authorization`, `Clearing`, `Refund`, `Reversal`, `Fee`
- `MCC`, `Merchant`, `MerchantDetails`, `EnhancedMerchantData`

### Financial Accounts and Statements

Financial accounts back the ledger. Statements summarize activity per billing period.

- `FinancialAccount`, `FinancialAccountDetails`
- `Statement`, `StatementDetails`, `StatementLine`
- `LoanTape`, `FinancialTransaction`, `ManagementOperation`

### Payments and Transfers

Lithic supports ACH payments, wire transfers, and internal book transfers.

- `Payment`, `PaymentDetails`
- `Transfer`, `TransferDetails`

### Authorization Rules

Auth rules let program managers approve or decline transactions based on card token, account token, program, merchant, or custom conditions.

- `AuthRule`, `AuthRuleDetails`, `Condition`

### Events and Webhooks

Every state change emits an event. Webhooks deliver events to customer endpoints.

- `Event`, `EventDetails`, `EventType`
- `Webhook`, `WebhookEvent`

### Program Management

Card programs group cards under a shared configuration (e.g., BIN, network, spend controls).

- `CardProgram`, `CardProgramDetails`

### API Keys and Tokens

- `APIKey` — management key for authentication
- `Token` — card network token (digitization in Apple Pay, Google Pay, etc.)
- `CardToken`, `CardMemo`

## Query Root

| Query | Description |
|---|---|
| `card(token: ID!)` | Fetch a single card by token |
| `cards(accountToken: ID, state: CardState)` | List cards with optional filters |
| `cardDetails(token: ID!)` | Sensitive card details (PAN/CVV) |
| `account(token: ID!)` | Fetch an account |
| `accountBalance(token: ID!)` | Current balance for an account |
| `transaction(token: ID!)` | Fetch a single transaction |
| `transactions(accountToken: ID, cardToken: ID, result: TransactionResult)` | List transactions |
| `authorization(token: ID!)` | Fetch an authorization event |
| `financialAccount(token: ID!)` | Fetch a financial account |
| `statement(token: ID!)` | Fetch a statement |
| `payment(token: ID!)` | Fetch a payment |
| `transfer(token: ID!)` | Fetch a transfer |
| `authRule(token: ID!)` | Fetch an auth rule |
| `authRules` | List all auth rules |
| `event(token: ID!)` | Fetch an event |
| `events(eventType: EventType)` | List events |
| `webhook(token: ID!)` | Fetch a webhook endpoint |
| `webhooks` | List webhook endpoints |
| `cardProgram(token: ID!)` | Fetch a card program |
| `kyc(accountHolderToken: ID!)` | Fetch KYC status for an individual |

## Mutation Root

| Mutation | Description |
|---|---|
| `createCard(input: CreateCardInput!)` | Issue a new virtual or physical card |
| `updateCard(token: ID!, input: UpdateCardInput!)` | Update card state, spend limit, or memo |
| `pauseCard(token: ID!)` | Pause card (sets state to PAUSED) |
| `closeCard(token: ID!)` | Permanently close a card |
| `createAccount(input: CreateAccountInput!)` | Create a new account |
| `updateAccountSpendLimit(token: ID!, input: SpendLimitInput!)` | Adjust account-level spend controls |
| `createPayment(input: CreatePaymentInput!)` | Initiate an ACH or wire payment |
| `createTransfer(input: CreateTransferInput!)` | Create a book transfer between financial accounts |
| `createAuthRule(input: CreateAuthRuleInput!)` | Create an authorization rule |
| `updateAuthRule(token: ID!, input: UpdateAuthRuleInput!)` | Update an existing auth rule |
| `applyAuthRule(token: ID!, cardTokens: [ID!], accountTokens: [ID!])` | Apply auth rule to cards or accounts |
| `createWebhook(input: CreateWebhookInput!)` | Register a webhook endpoint |
| `updateWebhook(token: ID!, input: UpdateWebhookInput!)` | Update a webhook URL or event types |
| `deleteWebhook(token: ID!)` | Remove a webhook endpoint |
| `submitKyc(input: KycInput!)` | Submit KYC data for an individual account holder |
| `submitKyb(input: KybInput!)` | Submit KYB data for a business account holder |

## Notes

- All monetary values are in the smallest currency unit (cents for USD).
- Card tokens, account tokens, and transaction tokens are UUIDs.
- Lithic uses cursor-based pagination; GraphQL connections use `after`/`first` arguments.
- Auth Stream Access (ASA) is a synchronous real-time webhook — not modeled as a GraphQL mutation.
- The `cardDetails` query requires elevated authentication scope.
