# Kuma (kuma)

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

Kuma is a platform-agnostic open-source service mesh built on top of Envoy proxy. It provides universal connectivity, security, and observability for services and microservices running on any infrastructure including Kubernetes and VMs.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/kuma/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/kuma/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Envoy
- Kubernetes
- Microservices
- Security
- Service Mesh

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-05-19

## APIs

### Kuma API

Kuma's control plane REST API for managing service mesh policies, dataplanes, zones, and configurations. It provides endpoints for inspecting and managing all mesh resources including traffic policies, service discovery, and health checks across Universal and Kubernetes deployments.

- **Human URL:** [https://kuma.io/docs/latest/reference/http-api/](https://kuma.io/docs/latest/reference/http-api/)
- **Base URL:** `https://localhost:5681`

#### Tags

- Control Plane
- Management
- REST API
- Service Mesh

#### Properties

- [Documentation](https://kuma.io/docs/latest/reference/http-api/)
- [Getting Started](https://kuma.io/docs/latest/installation/)
- [Reference](https://kuma.io/docs/latest/reference/http-api/)
- [OpenAPI](openapi/kuma-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kuma-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kuma-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/kuma-mesh-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Kuma Kubernetes Policy API

Kuma extends the Kubernetes API server with Custom Resource Definitions (CRDs) for defining and managing service mesh policies. These resources include MeshTrafficPermission, MeshRetry, MeshTimeout, MeshCircuitBreaker, MeshHealthCheck, MeshFaultInjection, and MeshRateLimit, enabling fine-grained traffic management, security, and resilience policies for meshed workloads.

- **Human URL:** [https://kuma.io/docs/latest/policies/](https://kuma.io/docs/latest/policies/)

#### Tags

- CRD
- Kubernetes
- Policy
- Traffic Management

#### Properties

- [Documentation](https://kuma.io/docs/latest/policies/)
- [Reference](https://kuma.io/docs/latest/reference/kubernetes-annotations/)
- [Postman Collection](collections/kuma-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kuma-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kuma Multizone API

Kuma's Multizone deployment API enables managing service meshes across multiple Kubernetes clusters and Universal zones from a single global control plane. It provides resources for zone management, cross-zone traffic routing, and zone egress and ingress configuration.

- **Human URL:** [https://kuma.io/docs/latest/production/deployment/multi-zone/](https://kuma.io/docs/latest/production/deployment/multi-zone/)

#### Tags

- Control Plane
- Federation
- Multi-Cluster
- Multizone

#### Properties

- [Documentation](https://kuma.io/docs/latest/production/deployment/multi-zone/)
- [Reference](https://kuma.io/docs/latest/reference/http-api/)
- [Postman Collection](collections/kuma-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kuma-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://kuma.io/)
- [Documentation](https://kuma.io/docs/)
- [Getting Started](https://kuma.io/docs/latest/installation/)
- [GitHub Organization](https://github.com/kumahq)
- [GitHub Repository](https://github.com/kumahq/kuma)
- [Community](https://kuma.io/community/)
- [Blog](https://kuma.io/blog/)
- [Slack](https://kuma-mesh.slack.com/)
- [Changelog](https://github.com/kumahq/kuma/releases)
- [Support](https://kuma.io/community/)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/kuma)
- [Security](https://github.com/kumahq/kuma/blob/master/SECURITY.md)
- [YouTube](https://www.youtube.com/@KumaMesh)
- [JSON Schema](json-schema/kuma-mesh-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/kuma-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
