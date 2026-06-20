# Turnkey (turnkey)

Turnkey is secure wallet infrastructure and a key-management / signing platform for crypto. Its API-first platform runs private key generation and signing inside verifiable secure enclaves (TEEs), exposing an RPC-style REST API for organizations and sub-organizations, wallets and wallet accounts, raw private keys, users, policies, and authenticators. Every request is cryptographically stamped (P-256 / API-key or passkey signature) and verified before execution.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/apis.yml)

## Tags

- Crypto
- Wallets
- Key Management
- Signing
- Secure Enclaves

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Turnkey Organizations & Sub-Organizations API

Create and manage the root organization and isolated sub-organizations, each with their own root quorum, users, policies, and wallets. The primary multi-tenant primitive for embedding wallets per end user.

- **Human URL:** [https://docs.turnkey.com/concepts/organizations](https://docs.turnkey.com/concepts/organizations)
- **Base URL:** `https://api.turnkey.com/public/v1`

#### Tags

- Organizations
- Sub-Organizations
- Tenancy

#### Properties

- [Documentation](https://docs.turnkey.com/concepts/sub-organizations)
- [API Reference](https://docs.turnkey.com/api-reference/activities/create-sub-organization)
- [OpenAPI](openapi/turnkey-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/turnkey.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/turnkey.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Turnkey Wallets API

Create HD wallets and derive multi-chain wallet accounts across secp256k1, ed25519, and P-256 curves (Ethereum, Bitcoin, Solana, and more), plus import and export of seed phrases inside the secure enclave.

- **Human URL:** [https://docs.turnkey.com/concepts/wallets](https://docs.turnkey.com/concepts/wallets)
- **Base URL:** `https://api.turnkey.com/public/v1`

#### Tags

- Wallets
- Wallet Accounts
- HD Wallets

#### Properties

- [Documentation](https://docs.turnkey.com/concepts/wallets)
- [API Reference](https://docs.turnkey.com/api-reference/activities/create-wallet)
- [OpenAPI](openapi/turnkey-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/turnkey.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/turnkey.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Turnkey Private Keys API

Generate, tag, import, and export standalone raw private keys managed inside Turnkey's secure enclaves, independent of HD wallet derivation, with curve and address-format selection.

- **Human URL:** [https://docs.turnkey.com/concepts/private-keys](https://docs.turnkey.com/concepts/private-keys)
- **Base URL:** `https://api.turnkey.com/public/v1`

#### Tags

- Private Keys
- Import
- Export

#### Properties

- [Documentation](https://docs.turnkey.com/concepts/private-keys)
- [API Reference](https://docs.turnkey.com/api-reference/activities/create-private-keys)
- [OpenAPI](openapi/turnkey-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/turnkey.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/turnkey.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Turnkey Signing & Activities API

Sign transactions and raw payloads (sign_transaction, sign_raw_payload, sign_raw_payloads) with a wallet account or private key, policy-checked and executed as activities; query activity status and results.

- **Human URL:** [https://docs.turnkey.com/api-reference/activities/overview](https://docs.turnkey.com/api-reference/activities/overview)
- **Base URL:** `https://api.turnkey.com/public/v1`

#### Tags

- Signing
- Transactions
- Activities

#### Properties

- [Documentation](https://docs.turnkey.com/concepts/policies/overview)
- [API Reference](https://docs.turnkey.com/api-reference/activities/sign-transaction)
- [OpenAPI](openapi/turnkey-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/turnkey.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/turnkey.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Turnkey Users, Policies & Authenticators API

Manage users, API keys, passkey/WebAuthn authenticators, OAuth providers, and the policy engine that authorizes every signing and administrative activity against the organization's root quorum.

- **Human URL:** [https://docs.turnkey.com/concepts/users/introduction](https://docs.turnkey.com/concepts/users/introduction)
- **Base URL:** `https://api.turnkey.com/public/v1`

#### Tags

- Users
- Policies
- Authenticators

#### Properties

- [Documentation](https://docs.turnkey.com/concepts/policies/overview)
- [API Reference](https://docs.turnkey.com/api-reference/activities/create-policies)
- [OpenAPI](openapi/turnkey-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/turnkey.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/turnkey.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/tkhq)
- [LinkedIn](https://www.linkedin.com/company/turnkeyhq)
- [Website](https://www.turnkey.com)
- [Documentation](https://docs.turnkey.com)
- [Plans](plans/turnkey-plans-pricing.yml)
- [Rate Limits](rate-limits/turnkey-rate-limits.yml)
- [Fin Ops](finops/turnkey-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
