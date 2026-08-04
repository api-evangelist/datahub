# DataHub (datahub)

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
