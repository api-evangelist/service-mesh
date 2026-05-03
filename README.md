# Service Mesh

**URL:** [https://raw.githubusercontent.com/api-evangelist/service-mesh/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/service-mesh/refs/heads/main/apis.yml)

Service mesh is a dedicated infrastructure layer for handling service-to-service communication in microservices architectures. It provides traffic management, mutual TLS security, observability, policy enforcement, and resilience features without requiring changes to application code. This index tracks service mesh specifications, implementations, and related APIs across the ecosystem including Istio, Linkerd, Consul Connect, AWS App Mesh, and the SMI standard.

## Timestamps

- **Created:** 2026-03-27
- **Modified:** 2026-05-02

## APIs

### Istio API

Istio is the most widely deployed service mesh. Istio's control plane exposes APIs for traffic management (VirtualService, DestinationRule, Gateway), security (PeerAuthentication, AuthorizationPolicy), and telemetry configuration via Kubernetes CRDs.

**Human URL:** [https://istio.io/latest/docs/reference/config/](https://istio.io/latest/docs/reference/config/)

#### Tags

Service Mesh, Istio, Traffic Management, Kubernetes, mTLS

---

### Linkerd Admin API

Linkerd is a lightweight CNCF-graduated service mesh focused on simplicity and security. Linkerd exposes an admin API for metrics, health checks, and edge proxy management. It uses the SMI API for traffic policy.

**Human URL:** [https://linkerd.io/2.14/reference/](https://linkerd.io/2.14/reference/)

#### Tags

Service Mesh, Linkerd, CNCF, Observability, mTLS

---

### Consul Connect / Service Mesh API

HashiCorp Consul provides service discovery and a service mesh (Consul Connect) with mutual TLS, intentions-based access control, and multi-datacenter support via a comprehensive REST API.

**Human URL:** [https://developer.hashicorp.com/consul/api-docs](https://developer.hashicorp.com/consul/api-docs)

#### Tags

Service Mesh, Consul, HashiCorp, Service Discovery, Zero Trust

---

### AWS App Mesh API

AWS App Mesh is a managed service mesh providing application-level networking for microservices on AWS, integrating with ECS, EKS, EC2, and Fargate.

**Human URL:** [https://docs.aws.amazon.com/app-mesh/latest/APIReference/](https://docs.aws.amazon.com/app-mesh/latest/APIReference/)

#### Tags

Service Mesh, AWS, Cloud, EKS, ECS

---

### Service Mesh Interface (SMI)

SMI is a standard interface for service meshes on Kubernetes defining common APIs for traffic policy, traffic telemetry, and traffic management, hosted by the CNCF.

**Human URL:** [https://smi-spec.io/](https://smi-spec.io/)

#### Tags

Service Mesh, SMI, Standard, Kubernetes, CNCF

---

## Common Properties

- [CNCF Landscape](https://landscape.cncf.io/guide#orchestration-management--service-mesh)
- [SMI Standard](https://smi-spec.io/)
- [Istio Documentation](https://istio.io/latest/docs/)
- [Linkerd Getting Started](https://linkerd.io/2.14/getting-started/)

## Artifacts

### JSON Schemas

| File | Description |
|------|-------------|
| [service-mesh-configuration-schema.json](json-schema/service-mesh-configuration-schema.json) | Abstract schema for common service mesh configuration primitives |

### JSON Structures

| File | Description |
|------|-------------|
| [service-mesh-traffic-policy-structure.json](json-structure/service-mesh-traffic-policy-structure.json) | Structural documentation for traffic policy primitives |

### JSON-LD Context

| File | Description |
|------|-------------|
| [service-mesh-context.jsonld](json-ld/service-mesh-context.jsonld) | JSON-LD context mapping service mesh vocabulary to schema.org |

### Examples

| File | Description |
|------|-------------|
| [service-mesh-traffic-split-example.json](examples/service-mesh-traffic-split-example.json) | Canary deployment traffic split using SMI TrafficSplit API |
| [service-mesh-mtls-example.json](examples/service-mesh-mtls-example.json) | Strict mutual TLS PeerAuthentication using Istio |

### Vocabulary

| File | Description |
|------|-------------|
| [service-mesh-vocabulary.yml](vocabulary/service-mesh-vocabulary.yml) | Domain vocabulary for service mesh concepts and patterns |

## Maintainers

**Email:** kin@apievangelist.com
