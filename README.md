# Tazama (tazama)

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
