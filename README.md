# Tazama

Tazama is the first open source platform for real-time financial monitoring and fraud detection, launched by Linux Foundation Charities with support from the Bill and Melinda Gates Foundation. It provides real-time fraud management, AML compliance, and cost-effective monitoring of digital financial transactions through a microservices architecture with rule processors, typology scoring, and case management integration. Built to ISO 20022 standards for maximum financial messaging interoperability.

**Website:** [https://tazama.org](https://tazama.org)  
**GitHub:** [https://github.com/tazama-lf](https://github.com/tazama-lf)  
**Documentation:** [https://tazama.org/products/](https://tazama.org/products/)

## APIs

### Tazama Transaction Monitoring Service API

The core API for ingesting real-time ISO 20022 financial transaction messages into the Tazama platform for fraud detection and AML compliance. Accepts pain.001, pain.013, pacs.008, and pacs.002 message types.

- **Base URL:** `http://localhost:5000`
- **OpenAPI:** [openapi/tazama-transaction-monitoring-service-openapi.yml](openapi/tazama-transaction-monitoring-service-openapi.yml)

#### Endpoints

| Method | Path | Summary |
|--------|------|---------|
| GET | `/` | Get Service Status |
| GET | `/health` | Get Health Status |
| POST | `/v1/evaluate/iso20022/pain.001.001.11` | Evaluate Pain 001 Transaction |
| POST | `/v1/evaluate/iso20022/pain.013.001.09` | Evaluate Pain 013 Transaction |
| POST | `/v1/evaluate/iso20022/pacs.008.001.10` | Evaluate Pacs 008 Transaction |
| POST | `/v1/evaluate/iso20022/pacs.002.001.12` | Evaluate Pacs 002 Transaction |

### Tazama Admin Service API

Administrative API for managing and configuring the Tazama platform including rule processors, typology definitions, and network maps.

- **Base URL:** `http://localhost:5100`
- **GitHub:** [https://github.com/tazama-lf/admin-service](https://github.com/tazama-lf/admin-service)

## Features

- **Real-Time Transaction Monitoring** - Processes financial transactions in real time for immediate fraud detection
- **ISO 20022 Compliance** - Built to ISO 20022 standards for financial messaging interoperability
- **Payment Platform Adapter** - Transforms non-ISO 20022 messages into compatible formats
- **Rule-Based Fraud Detection** - Configurable rule processors evaluate transactions for suspicious behavior
- **Typology Scoring** - Aggregates rule results into fraud and AML typology scores
- **AML Compliance** - Anti-money laundering monitoring built into the processing pipeline
- **Case Management Integration** - Issues investigation alerts to external case management systems
- **Transaction Blocking** - Can block high-risk transactions to prevent financial loss
- **Kubernetes Deployment** - Helm charts available for AKS, EKS, GKE, and on-premises deployments
- **GraphQL Access** - Hasura GraphQL API layer for flexible database queries

## Use Cases

- **Fraud Detection for Mobile Money Operators** - Real-time monitoring of mobile financial transactions
- **AML Compliance for Banks** - Automated AML screening to meet regulatory requirements
- **Payment Switch Monitoring** - Monitor transactions through payment switches
- **Clearing House Risk Management** - Screen clearing house transactions for fraud and money laundering

## Artifacts

### OpenAPI Specifications

| File | Description |
|------|-------------|
| [openapi/tazama-transaction-monitoring-service-openapi.yml](openapi/tazama-transaction-monitoring-service-openapi.yml) | Transaction Monitoring Service API |

### Naftiko Capabilities

| File | Description |
|------|-------------|
| [capabilities/fraud-detection.yaml](capabilities/fraud-detection.yaml) | Real-time fraud detection workflow capability |
| [capabilities/shared/transaction-monitoring.yaml](capabilities/shared/transaction-monitoring.yaml) | Shared TMS API consumed definition |

### Spectral Rules

| File | Description |
|------|-------------|
| [rules/tazama-rules.yml](rules/tazama-rules.yml) | Spectral ruleset for Tazama API conventions |

### JSON Schemas

| File | Description |
|------|-------------|
| [json-schema/tazama-transaction-response-schema.json](json-schema/tazama-transaction-response-schema.json) | Transaction evaluation response schema |
| [json-schema/tazama-iso20022-pain001-schema.json](json-schema/tazama-iso20022-pain001-schema.json) | ISO 20022 pain.001.001.11 message schema |

### JSON Structures

| File | Description |
|------|-------------|
| [json-structure/tazama-transaction-response-structure.json](json-structure/tazama-transaction-response-structure.json) | Transaction response field documentation |

### JSON-LD Context

| File | Description |
|------|-------------|
| [json-ld/tazama-context.jsonld](json-ld/tazama-context.jsonld) | Linked data context for Tazama vocabulary |

### Examples

| File | Description |
|------|-------------|
| [examples/tazama-evaluate-pain001-transaction-example.json](examples/tazama-evaluate-pain001-transaction-example.json) | pain.001 transaction evaluation example |
| [examples/tazama-evaluate-pacs008-transaction-example.json](examples/tazama-evaluate-pacs008-transaction-example.json) | pacs.008 transfer evaluation example |

### Vocabulary

| File | Description |
|------|-------------|
| [vocabulary/tazama-vocabulary.yml](vocabulary/tazama-vocabulary.yml) | Tazama domain terminology and definitions |

## Integrations

- **Hasura GraphQL** - GraphQL access layer to the Tazama database
- **Keycloak** - Identity and access management
- **NATS** - Event streaming for inter-service communication
- **ArangoDB** - Multi-model database for transaction data
- **Mojaloop** - ISO 20022 message mapping for Mojaloop financial network

## License

Apache 2.0 - Linux Foundation Charities

## Maintainers

**FN:** Kin Lane  
**Email:** info@apievangelist.com
