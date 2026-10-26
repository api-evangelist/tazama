# Tazama (tazama)

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

Tazama is the first open source platform for real-time financial monitoring and fraud detection, launched by Linux Foundation Charities with support from the Bill and Melinda Gates Foundation. It provides real-time fraud management, AML compliance, and cost-effective monitoring of digital financial transactions through a microservices architecture with rule processors, typology scoring, and case management integration. Built to ISO 20022 standards for maximum financial messaging interoperability.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Financial Technology
- Fraud Detection
- Anti-Money Laundering
- Linux Foundation
- Open Source
- Transaction Monitoring
- ISO 20022
- Real Time

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-05-19

## APIs

### Tazama Transaction Monitoring Service API

The core API for ingesting real-time ISO 20022 financial transaction messages into the Tazama platform for fraud detection and AML compliance. Accepts pain.001, pain.013, pacs.008, and pacs.002 message types from financial service providers including banks, remitters, mobile money operators, clearing houses, and payment switches. Validates messages, routes them through configurable rule processors, and returns fraud and AML evaluation results.

- **Human URL:** [https://tazama.org/products/](https://tazama.org/products/)
- **Base URL:** `http://localhost:5000`

#### Tags

- Transaction Monitoring
- ISO 20022
- Fraud Detection
- Real Time

#### Properties

- [Documentation](https://tazama.org/products/)
- [GitHub Repository](https://github.com/tazama-lf/tms-service)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/openapi/tazama-transaction-monitoring-service-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tazama-transaction-monitoring-service.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tazama-transaction-monitoring-service.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tazama Admin Service API

Administrative API for managing and configuring the Tazama platform. Supports configuration of rule processors, typology definitions, network maps, and system administration. Swagger documentation available at the admin service endpoint.

- **Human URL:** [https://github.com/tazama-lf/admin-service](https://github.com/tazama-lf/admin-service)
- **Base URL:** `http://localhost:5100`

#### Tags

- Administration
- Configuration
- Rule Management

#### Properties

- [Documentation](https://github.com/tazama-lf/admin-service)
- [GitHub Repository](https://github.com/tazama-lf/admin-service)
- [Postman Collection](collections/tazama-transaction-monitoring-service.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tazama-transaction-monitoring-service.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/tazama-org)
- [Documentation](https://tazama.org/products/)
- [Git Hub Org](https://github.com/tazama-lf)
- [About](https://tazama.org/about/)
- [Licensing](https://www.linuxfoundation.org/press/linux-foundation-launches-tazama-for-real-time-fraud-management)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/openapi/tazama-transaction-monitoring-service-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/vocabulary/tazama-vocabulary.yml)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/json-schema/tazama-transaction-response-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [J S O N L D Context](https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/json-ld/tazama-context.jsonld)
- [Spectral Rules](https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/rules/tazama-rules.yml)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
