# Turnkey (turnkey)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
