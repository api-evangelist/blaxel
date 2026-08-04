# Blaxel (blaxel)

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

Blaxel (formerly Beamlit) is an infrastructure and compute platform built for AI agents. Its control plane API deploys and manages agents, MCP/function servers, serverless code sandboxes, batch jobs, a multi-provider model gateway, deployment policies, integrations, and multi-tenant workspaces. The REST control plane lives at api.blaxel.ai/v0 and authenticates with a Bearer API key or OAuth 2.0.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/apis.yml)

> **State note:** Blaxel was formerly named **Beamlit** and rebranded to Blaxel. Residual "Beamlit" naming still appears in some GitHub repositories. The active brand and surfaces are Blaxel — blaxel.ai, docs.blaxel.ai, api.blaxel.ai, and the [blaxel-ai](https://github.com/blaxel-ai) GitHub organization.

## Tags

- AI
- Agents
- Infrastructure
- Sandboxes
- MCP
- Compute
- Serverless

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### Blaxel Agents API

Deploy, list, update, and delete AI agents as serverless auto-scaling HTTP endpoints, with revision history. Framework-agnostic - bring your own code (LangChain, CrewAI, Claude Agent SDK) and Blaxel builds and runs it.

- **Human URL:** [https://docs.blaxel.ai/Agents/Overview](https://docs.blaxel.ai/Agents/Overview)
- **Base URL:** `https://api.blaxel.ai/v0`

#### Tags

- Agents
- Deployments
- Serverless

#### Properties

- [Documentation](https://docs.blaxel.ai/Agents/Overview)
- [API Reference](https://docs.blaxel.ai/api-reference/agents)
- [OpenAPI](openapi/blaxel-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/blaxel.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/blaxel.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Blaxel Functions / MCP Servers API

Deploy custom MCP (Model Context Protocol) tool servers as fast-starting serverless endpoints that extend agents' capabilities, with built-in authentication, rate limiting, and observability. Managed as functions with revision history.

- **Human URL:** [https://docs.blaxel.ai/Functions/Overview](https://docs.blaxel.ai/Functions/Overview)
- **Base URL:** `https://api.blaxel.ai/v0`

#### Tags

- Functions
- MCP
- Tools

#### Properties

- [Documentation](https://docs.blaxel.ai/Functions/Overview)
- [API Reference](https://docs.blaxel.ai/api-reference/functions)
- [OpenAPI](openapi/blaxel-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/blaxel.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/blaxel.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Blaxel Models Gateway API

Register and manage model deployments that front an intelligent routing layer to LLM providers, with built-in telemetry, token cost control, and fallback. A single gateway endpoint proxies inference to the configured upstream provider.

- **Human URL:** [https://docs.blaxel.ai/Models/Overview](https://docs.blaxel.ai/Models/Overview)
- **Base URL:** `https://api.blaxel.ai/v0`

#### Tags

- Models
- Model Gateway
- Inference
- Routing

#### Properties

- [Documentation](https://docs.blaxel.ai/Models/Overview)
- [API Reference](https://docs.blaxel.ai/api-reference/models)
- [OpenAPI](openapi/blaxel-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/blaxel.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/blaxel.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Blaxel Sandboxes API

Create, start, stop, and delete secure microVM sandboxes that boot from standby in under 25ms, exposing filesystem, process, and code execution for agent runtimes. Includes sandbox previews and scoped preview tokens for shareable URLs.

- **Human URL:** [https://docs.blaxel.ai/Sandboxes/Overview](https://docs.blaxel.ai/Sandboxes/Overview)
- **Base URL:** `https://api.blaxel.ai/v0`

#### Tags

- Sandboxes
- Compute
- Code Execution
- MicroVM

#### Properties

- [Documentation](https://docs.blaxel.ai/Sandboxes/Overview)
- [API Reference](https://docs.blaxel.ai/api-reference/compute)
- [OpenAPI](openapi/blaxel-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/blaxel.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/blaxel.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Blaxel Jobs API

Define and run asynchronous batch jobs for extended workloads (up to 24 hours) of background processing at scale, and manage their executions and revisions.

- **Human URL:** [https://docs.blaxel.ai/Jobs/Overview](https://docs.blaxel.ai/Jobs/Overview)
- **Base URL:** `https://api.blaxel.ai/v0`

#### Tags

- Jobs
- Batch
- Async

#### Properties

- [Documentation](https://docs.blaxel.ai/Jobs/Overview)
- [API Reference](https://docs.blaxel.ai/api-reference/jobs)
- [OpenAPI](openapi/blaxel-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/blaxel.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/blaxel.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Blaxel Policies API

Create and manage deployment policies that constrain where and how workloads run - governing regions, flavors, and provider routing across environments.

- **Human URL:** [https://docs.blaxel.ai/Model-Governance/Policies](https://docs.blaxel.ai/Model-Governance/Policies)
- **Base URL:** `https://api.blaxel.ai/v0`

#### Tags

- Policies
- Governance
- Deployment

#### Properties

- [Documentation](https://docs.blaxel.ai/Model-Governance/Policies)
- [API Reference](https://docs.blaxel.ai/api-reference/policies)
- [OpenAPI](openapi/blaxel-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/blaxel.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/blaxel.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Blaxel Integrations API

Manage integration connections to external providers (model providers, tool sources, code repositories), list connection-backed models, and read endpoint configurations that agents and the model gateway consume.

- **Human URL:** [https://docs.blaxel.ai/Integrations/Overview](https://docs.blaxel.ai/Integrations/Overview)
- **Base URL:** `https://api.blaxel.ai/v0`

#### Tags

- Integrations
- Connections
- Providers

#### Properties

- [Documentation](https://docs.blaxel.ai/Integrations/Overview)
- [API Reference](https://docs.blaxel.ai/api-reference/integrations)
- [OpenAPI](openapi/blaxel-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/blaxel.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/blaxel.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Blaxel Workspaces API

Create and manage multi-tenant workspaces, invite and manage users and roles, and administer service accounts and their API keys for programmatic access and IAM.

- **Human URL:** [https://docs.blaxel.ai/Security/Workspace-access-control](https://docs.blaxel.ai/Security/Workspace-access-control)
- **Base URL:** `https://api.blaxel.ai/v0`

#### Tags

- Workspaces
- IAM
- Multi-Tenant
- Service Accounts

#### Properties

- [Documentation](https://docs.blaxel.ai/Security/Workspace-access-control)
- [API Reference](https://docs.blaxel.ai/api-reference/workspaces)
- [OpenAPI](openapi/blaxel-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/blaxel.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/blaxel.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/blaxel-ai)
- [LinkedIn](https://www.linkedin.com/company/blaxel)
- [Website](https://blaxel.ai/)
- [Documentation](https://docs.blaxel.ai/)
- [Plans](plans/blaxel-plans-pricing.yml)
- [Rate Limits](rate-limits/blaxel-rate-limits.yml)
- [Fin Ops](finops/blaxel-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
