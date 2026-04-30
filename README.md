# DataHub (datahub)
DataHub is LinkedIn's generalized metadata search and discovery platform, providing a unified data catalog, lineage graph, governance tooling, and event-driven Actions Framework. It exposes GraphQL, OpenAPI, and Rest.li APIs along with Python and Java SDKs and a CLI for metadata ingestion.

**URL:** [Visit APIs.yml URL](https://raw.githubusercontent.com/api-evangelist/datahub/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party
- **xType:** opensource

## Tags

- Data Catalog, Data Discovery, Data Governance, Data Lineage, Metadata

## Timestamps

- **Created:** 2024-01-15
- **Modified:** 2026-04-28

## APIs

### DataHub GraphQL API
Primary API for querying and mutating metadata. Mirrors the capabilities of the DataHub UI.

### DataHub OpenAPI
RESTful endpoints for entities, relationships, timeline history, and platform events.

- [OpenAPI](openapi/datahub-openapi-openapi.yml)
- [JSONSchema](json-schema/datahub-metadata-change-log-event-schema.json)

### DataHub REST API
The Rest.li API representing the underlying persistence layer with raw PDL aspect models. Considered system-internal.

### DataHub Python SDK
The acryl-datahub package providing CLI and SDK with REST and Kafka emitter APIs for metadata ingestion.

### DataHub Java SDK
The io.acryl datahub-client package offering REST emitter APIs for JVM-based systems.

### DataHub CLI
Command line tool installed with the acryl-datahub Python package for ingestion, entity management, and administration.

### DataHub Actions Framework
Event-driven framework consuming Metadata Change Logs and Platform Events.

- [AsyncAPI](asyncapi/datahub-actions-asyncapi.yml)

## Common Properties

- [Website](https://datahub.com)
- [Documentation](https://docs.datahub.com/docs/)
- [GitHub Repository](https://github.com/datahub-project/datahub)
- [Slack](https://slack.datahubproject.io)
- [JSON-LD](json-ld/datahub-context.jsonld)
- [Vocabulary](vocabulary/datahub-vocabulary.yml)
- [Capabilities](capabilities/datahub-capabilities.yml)
- [Rules](rules/datahub-rules.yml)

## Maintainers

- **FN:** Kin Lane
- **Email:** kin@apievangelist.com
