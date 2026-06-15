# Kuma (kuma)

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
