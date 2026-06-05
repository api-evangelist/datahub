# DataHub (datahub)

DataHub is LinkedIn's generalized metadata search and discovery platform, providing a unified data catalog, lineage graph, governance tooling, and event-driven Actions Framework. It exposes GraphQL, OpenAPI, and Rest.li APIs along with Python and Java SDKs and a CLI for metadata ingestion.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/datahub/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/datahub/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Data Catalog
- Data Discovery
- Data Governance
- Data Lineage
- Metadata

## Timestamps

- **Created:** 2024-01-15
- **Modified:** 2026-05-19

## APIs

### DataHub GraphQL API

Primary API for querying and mutating metadata in DataHub. The GraphQL API serves as the main public API for the platform and can be used to fetch and update metadata programmatically in the language of your choice. It mirrors the capabilities available in the DataHub UI.

- **Human URL:** [https://docs.datahub.com/docs/api/graphql/overview](https://docs.datahub.com/docs/api/graphql/overview)
- **Base URL:** `http://localhost:8080/api/graphql`

#### Tags

- GraphQL
- Metadata
- Queries
- Search

#### Properties

- [Documentation](https://docs.datahub.com/docs/api/graphql/overview)
- [Getting Started](https://docs.datahub.com/docs/api/graphql/getting-started)
- [Reference](https://docs.datahub.com/docs/graphql/queries)
- [Playground](http://localhost:8080/api/graphiql)
- [Postman Collection](collections/datahub-openapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datahub-openapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DataHub OpenAPI

RESTful API endpoints documented using the OpenAPI standard for interacting with DataHub metadata. Provides endpoints for entities, relationships, timeline, and platform events. The OpenAPI spec is auto-generated and available via Swagger UI for interactive exploration. Recommended for advanced users who need lower-level access to the metadata graph.

- **Human URL:** [https://docs.datahub.com/docs/api/openapi/openapi-usage-guide](https://docs.datahub.com/docs/api/openapi/openapi-usage-guide)
- **Base URL:** `http://localhost:8080/openapi/`

#### Tags

- Entities
- Metadata
- OpenAPI
- REST

#### Properties

- [Documentation](https://docs.datahub.com/docs/api/openapi/openapi-usage-guide)
- [OpenAPI](openapi/datahub-openapi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/datahub-openapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datahub-openapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/datahub-metadata-change-log-event-schema.json) — [JSON Schema](https://json-schema.org/specification)

### DataHub REST API

The Rest.li API represents the underlying persistence layer and exposes the raw PDL models used in storage. It powers the GraphQL API under the hood and is used for system-specific ingestion of metadata by the Metadata Ingestion Framework. This API is considered system-internal and is not recommended for direct external use.

- **Human URL:** [https://docs.datahub.com/docs/api/datahub-apis](https://docs.datahub.com/docs/api/datahub-apis)
- **Base URL:** `http://localhost:8080/`

#### Tags

- Entities
- Internal
- Metadata
- REST

#### Properties

- [Documentation](https://docs.datahub.com/docs/api/datahub-apis)
- [Postman Collection](collections/datahub-openapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datahub-openapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DataHub Python SDK

Python client for interacting with DataHub. The acryl-datahub package provides a CLI and SDK for DataHub, including REST and Kafka emitter APIs for pushing metadata programmatically. It is one of the most recommended tools for extending and customizing DataHub behavior, especially for ingestion and bulk metadata operations.

- **Human URL:** [https://docs.datahub.com/docs/metadata-ingestion/as-a-library](https://docs.datahub.com/docs/metadata-ingestion/as-a-library)
- **Base URL:** `https://pypi.org/project/acryl-datahub/`

#### Tags

- Emitter
- Ingestion
- Python
- SDK

#### Properties

- [Documentation](https://docs.datahub.com/docs/metadata-ingestion/as-a-library)
- [GitHub Repository](https://github.com/datahub-project/datahub)
- [S D Ks](https://pypi.org/project/acryl-datahub/)
- [Postman Collection](collections/datahub-openapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datahub-openapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DataHub Java SDK

Java client for interacting with DataHub. The io.acryl datahub-client package offers REST emitter APIs that can be used to emit metadata from JVM-based systems. It supports all major DataHub entity types including Dataset, Chart, Dashboard, Container, DataFlow, DataJob, MLModel, and MLModelGroup.

- **Human URL:** [https://docs.datahub.com/docs/metadata-integration/java/as-a-library](https://docs.datahub.com/docs/metadata-integration/java/as-a-library)
- **Base URL:** `https://github.com/datahub-project/datahub`

#### Tags

- Emitter
- Java
- Metadata
- SDK

#### Properties

- [Documentation](https://docs.datahub.com/docs/metadata-integration/java/as-a-library)
- [GitHub Repository](https://github.com/datahub-project/datahub)
- [Postman Collection](collections/datahub-openapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datahub-openapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DataHub CLI

Command line tool for interacting with DataHub. The datahub CLI allows you to perform common operations including metadata ingestion, entity management, and system administration from the command line. It is installed as part of the acryl-datahub Python package and supports a plugin architecture for different data source connectors.

- **Human URL:** [https://docs.datahub.com/docs/cli](https://docs.datahub.com/docs/cli)
- **Base URL:** `https://pypi.org/project/acryl-datahub/`

#### Tags

- CLI
- Command Line
- Ingestion
- Metadata

#### Properties

- [Documentation](https://docs.datahub.com/docs/cli)
- [Getting Started](https://docs.datahub.com/docs/metadata-ingestion/cli-ingestion)
- [S D Ks](https://pypi.org/project/acryl-datahub/)
- [Postman Collection](collections/datahub-openapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datahub-openapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DataHub Actions Framework

Event-driven framework for responding to real-time changes in the DataHub metadata graph. The Actions Framework allows you to configure event sources, transformations, and actions using YAML configuration files. It enables seamless integration of DataHub into a broader event-based architecture by consuming Metadata Change Logs and Platform Events.

- **Human URL:** [https://docs.datahub.com/docs/actions](https://docs.datahub.com/docs/actions)
- **Base URL:** `https://pypi.org/project/acryl-datahub-actions/`

#### Tags

- Actions
- Automation
- Events
- Real-Time

#### Properties

- [Documentation](https://docs.datahub.com/docs/actions)
- [Getting Started](https://docs.datahub.com/docs/actions/quickstart)
- [S D Ks](https://pypi.org/project/acryl-datahub-actions/)
- [AsyncAPI](asyncapi/datahub-actions-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/datahub-openapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datahub-openapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Website](https://datahub.com)
- [Portal](https://docs.datahub.com)
- [Documentation](https://docs.datahub.com/docs/)
- [Getting Started](https://docs.datahub.com/docs/quickstart)
- [Authentication](https://docs.datahub.com/docs/authentication)
- [GitHub Repository](https://github.com/datahub-project/datahub)
- [Slack](https://slack.datahubproject.io)
- [Blog](https://datahub.com/blog/)
- [Demo](https://demo.datahubproject.io/)
- [Changelog](https://github.com/datahub-project/datahub/releases)
- [Status Page](https://status.datahub.com)
- [Community](https://forum.datahubproject.io/)
- [YouTube](https://youtube.com/@datahubproject)
- [LinkedIn](https://www.linkedin.com/company/datahub-cloud)
- [Privacy Policy](https://datahub.com/privacy-policy/)
- [Security](https://docs.datahub.com/docs/security_stance)
- [JSON-LD](json-ld/datahub-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/datahub-vocabulary.yml)
- [Capabilities](capabilities/datahub-capabilities.yml)
- [Rules](rules/datahub-rules.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
