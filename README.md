# DataHub

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

DataHub is LinkedIn's generalized metadata search and discovery platform, providing a unified data catalog, lineage graph, governance tooling, and event-driven Actions Framework. It exposes GraphQL, OpenAPI, and Rest.li APIs along with Python and Java SDKs and a CLI for metadata ingestion.

**Areas:** Data Catalog · Data Discovery · Data Governance · Data Lineage · Metadata · Real-Time

## DataHub on APIs.io

Everything profiled for DataHub is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/datahub/](https://apis.io/providers/datahub/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [DataHub GraphQL API](https://apis.io/apis/datahub/datahub-graphql-api/) — Primary API for querying and mutating metadata in DataHub. The GraphQL API serves as the main public API for the platform and can be used to fetch and…
- [DataHub REST API](https://apis.io/apis/datahub/datahub-rest-api/) — The Rest.li API represents the underlying persistence layer and exposes the raw PDL models used in storage. It powers the GraphQL API under the hood and is…
- [DataHub Python SDK](https://apis.io/apis/datahub/datahub-python-sdk/) — Python client for interacting with DataHub. The acryl-datahub package provides a CLI and SDK for DataHub, including REST and Kafka emitter APIs for pushing…
- [DataHub Java SDK](https://apis.io/apis/datahub/datahub-java-sdk/) — Java client for interacting with DataHub. The io.acryl datahub-client package offers REST emitter APIs that can be used to emit metadata from JVM-based…
- [DataHub CLI](https://apis.io/apis/datahub/datahub-cli/) — Command line tool for interacting with DataHub. The datahub CLI allows you to perform common operations including metadata ingestion, entity management, and…
- [DataHub Actions Framework](https://apis.io/apis/datahub/datahub-actions-framework/) — Event-driven framework for responding to real-time changes in the DataHub metadata graph. The Actions Framework allows you to configure event sources,…
- [DataHub Batch API](https://apis.io/apis/datahub/datahub-batch-api/) — Batch operations for fetching multiple entities and their aspects in a single request. Supports version-specific retrieval and conditional writes.
- [DataHub Entities API](https://apis.io/apis/datahub/datahub-entities-api/) — Read, write, and delete metadata entities in the DataHub metadata graph. The entities endpoints support upserting entity-aspect pairs, retrieving the latest…
- [DataHub Platform API](https://apis.io/apis/datahub/datahub-platform-api/) — Write metadata events using the standard platform format. Provides an alternative ingestion path for emitting metadata change proposals to the DataHub…
- [DataHub Relationships API](https://apis.io/apis/datahub/datahub-relationships-api/) — Query the relationship graph to navigate connections between entities. Supports filtering by relationship type and traversal direction (incoming or…
- [DataHub Timeline API](https://apis.io/apis/datahub/datahub-timeline-api/) — Query the versioned history of entity aspects over time. Useful for tracking schema changes, documentation updates, and other temporal metadata…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (7)

Multi-step workflows that chain operations into a business task.

- [DataHub Add Glossary Terms to a Dataset](https://apis.io/arazzos/datahub/datahub-add-glossary-terms-workflow/)
- [DataHub Assign Dataset Ownership](https://apis.io/arazzos/datahub/datahub-assign-ownership-workflow/)
- [DataHub Decommission a Dataset](https://apis.io/arazzos/datahub/datahub-decommission-dataset-workflow/)
- [DataHub Emit Platform Event and Audit](https://apis.io/arazzos/datahub/datahub-emit-and-audit-workflow/)
- [DataHub Tag a Dataset](https://apis.io/arazzos/datahub/datahub-tag-dataset-workflow/)
- [DataHub Trace Dataset Lineage](https://apis.io/arazzos/datahub/datahub-trace-lineage-workflow/)
- [DataHub Upsert Dataset and Verify](https://apis.io/arazzos/datahub/datahub-upsert-dataset-workflow/)

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [DataHub Actions Framework Events](https://apis.io/asyncapis/datahub/datahub-actions-asyncapi/)

#### Event channels (3)

Individual events and webhooks the provider emits.

- [MetadataChangeLog_Timeseries_v1](https://apis.io/channels/datahub/metadatachangelog-timeseries-v1/)
- [MetadataChangeLog_Versioned_v1](https://apis.io/channels/datahub/metadatachangelog-versioned-v1/)
- [PlatformEvent_v1](https://apis.io/channels/datahub/platformevent-v1/)

#### GraphQL (1)

GraphQL schemas.

- [DataHub GraphQL API](https://apis.io/graphqls/datahub/datahub-graphql/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [datahub](https://apis.io/servers/datahub/datahub/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Datahub Agentic Access](https://apis.io/agentic-access/datahub/datahub-agentic-access/)

#### JSON Schema (14)

The data models the API reads and writes.

- [AspectValue](https://apis.io/schemas/datahub/datahub-aspectvalue/)
- [AuditStamp](https://apis.io/schemas/datahub/datahub-auditstamp/)
- [BatchGetRequest](https://apis.io/schemas/datahub/datahub-batchgetrequest/)
- [ChangeEvent](https://apis.io/schemas/datahub/datahub-changeevent/)
- [ChangeTransaction](https://apis.io/schemas/datahub/datahub-changetransaction/)
- [EntityAspectRequest](https://apis.io/schemas/datahub/datahub-entityaspectrequest/)
- [EntityAspectResponse](https://apis.io/schemas/datahub/datahub-entityaspectresponse/)
- [Error](https://apis.io/schemas/datahub/datahub-error/)
- [DataHub Metadata Change Log Event](https://apis.io/schemas/datahub/datahub-metadata-change-log-event/)
- [MetadataChangeProposal](https://apis.io/schemas/datahub/datahub-metadatachangeproposal/)
- [Relationship](https://apis.io/schemas/datahub/datahub-relationship/)
- [RelationshipsResponse](https://apis.io/schemas/datahub/datahub-relationshipsresponse/)
- [SystemMetadata](https://apis.io/schemas/datahub/datahub-systemmetadata/)
- [TimelineResponse](https://apis.io/schemas/datahub/datahub-timelineresponse/)

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Datahub Structure](https://apis.io/json-structure/datahub/datahub-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Datahub Context](https://apis.io/jsonld/datahub/datahub-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [DataHub Vocabulary](https://apis.io/vocabularies/datahub/datahub-vocabulary/)

#### Collections (7)

Postman and Open Collection request collections.

- [DataHub Open Batch API](https://apis.io/collections/datahub/open-datahub-batch-api/)
- [DataHub Open Batch Entities API](https://apis.io/collections/datahub/open-datahub-entities-api/)
- [DataHub OpenAPI](https://apis.io/collections/datahub/open-datahub-openapi/)
- [DataHub Open Batch Platform API](https://apis.io/collections/datahub/open-datahub-platform-api/)
- [DataHub Open Batch Relationships API](https://apis.io/collections/datahub/open-datahub-relationships-api/)
- [DataHub Open Batch Timeline API](https://apis.io/collections/datahub/open-datahub-timeline-api/)
- [DataHub OpenAPI](https://apis.io/collections/datahub/postman-datahub-openapi/)

#### Governance rules (3)

Spectral rulesets for the provider's contracts.

- [DataHub — asyncapi rules](https://apis.io/rules/datahub/datahub-asyncapi-spectral-rules/)
- [DataHub — jsonschema rules](https://apis.io/rules/datahub/datahub-jsonschema-spectral-rules/)
- [DataHub API Rules](https://apis.io/rules/datahub/datahub-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Datahub Authentication](https://apis.io/security/datahub/datahub-authentication/)
- [Datahub Domain Security](https://apis.io/security/datahub/datahub-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Datahub Plans Pricing](https://apis.io/plans/datahub/datahub-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Datahub Rate Limits](https://apis.io/rate-limits/datahub/datahub-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Datahub Finops](https://apis.io/finops/datahub/datahub-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://datahub.com)
- [Documentation](https://docs.datahub.com/docs/)
- [Getting started](https://docs.datahub.com/docs/quickstart)
- [Changelog](https://github.com/datahub-project/datahub/releases)
- [Blog](https://datahub.com/blog/)
- [Security](https://docs.datahub.com/docs/security_stance)
- [Privacy policy](https://datahub.com/privacy-policy/)
- [Status](https://status.datahub.com)

## API Evangelist rating

**Kin Score 55.6** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 60.0 |
| Contract quality | 61.8 |
| Contract governance | 27.3 |
| Operational transparency | 52.6 |
| Developer ergonomics | 66.7 |
| Access clarity | 15.8 |

**Agent readiness 48.9** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | derived (partial credit) |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 20.6** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/datahub/](https://apis.io/providers/datahub/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for DataHub: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/datahub/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
