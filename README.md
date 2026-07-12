# ARMO (armosec)

ARMO is the cloud-native and Kubernetes security company behind the leading open-source project **Kubescape**. ARMO Platform is a runtime-driven CNAPP that unifies Kubernetes Security Posture Management (KSPM), vulnerability and image scanning, compliance frameworks, network and seccomp policy generation, and runtime **Cloud Application Detection and Response (CADR)** — correlating in-cluster runtime behavior with posture and vulnerability data to cut alert noise and surface exploitable attack chains.

ARMO exposes a **documented REST API** over HTTPS. Requests go to a regional base URL — `https://api.armosec.io/api/v1` (EU) or `https://api.us.armosec.io/api/v1` (US) — and are authenticated with an account **access key** (Agent Access Key) sent in the `X-API-KEY` header. Interactive docs are available at `https://api.armosec.io/openapi/v2/swaggerui` (Swagger UI), `/rapi` (RapiDoc), and `/docs` (ReDoc).

**Access model:** The API surface and its OpenAPI/Swagger are publicly documented, but the API is operationally **account-gated**. Calls require an access key generated in ARMO Platform, and meaningful data requires a connected account with reporting Kubernetes clusters (via the Kubescape/ARMO Helm-deployed operator) or connected registries and repositories. There is no anonymous public data endpoint. The endpoint list in this catalog is honestly modeled from ARMO's public API reference and Swagger; verify exact request/response payloads against the live Swagger UI.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/apis.yml)

## Tags

- Kubernetes Security
- Cloud Native Security
- CNAPP
- DevSecOps
- KSPM
- Vulnerability Management
- Compliance
- Runtime Security
- CADR
- Kubescape
- Container Security

## Timestamps

- **Created:** 2026-07-11
- **Modified:** 2026-07-11

## APIs

### ARMO Vulnerabilities API

Query image and workload vulnerabilities. Issue scans for a workload or context, retrieve scan-result summaries and details, severity roll-ups, top vulnerabilities, and vulnerability lists scoped by component or image, and manage vulnerability exceptions.

- **Base URL:** `https://api.armosec.io/api/v1`
- Tags: Vulnerabilities, CVE, Image Scanning, Kubernetes Security

### ARMO Posture and Compliance API

KSPM results across compliance frameworks. Get per-framework scan summaries, control run results and framework sections, affected resources, repository (IaC) posture reports, and manage posture exceptions.

- **Base URL:** `https://api.armosec.io/api/v1`
- Tags: Compliance, KSPM, Posture, Cloud Native Security

### ARMO Clusters and Workloads API

Inventory of connected Kubernetes clusters and workloads. Retrieve the cluster list with history over time, list workloads with their vulnerability and posture context, and check onboarding and scan report state.

- **Base URL:** `https://api.armosec.io/api/v1`
- Tags: Clusters, Workloads, Kubernetes Security

### ARMO Runtime Incidents API

Runtime CADR. List runtime incidents and their alerts, get an incident explanation, resolve/unresolve incidents, and get incidents grouped by severity — built on ARMO's eBPF runtime sensor.

- **Base URL:** `https://api.armosec.io/api/v1`
- Tags: Runtime Security, CADR, Threat Detection, Incidents

### ARMO Security Risks and Attack Chains API

Prioritized, correlated security risks and attack chains. List security risks, associated resources, and severity summaries, and retrieve attack chains that combine posture, vulnerability, and runtime signals into exploitable paths.

- **Base URL:** `https://api.armosec.io/api/v1`
- Tags: Security Risks, Attack Path, CNAPP, Cloud Native Security

### ARMO Network and Runtime Policies API

Generate and manage hardening policies from observed runtime behavior. Retrieve and generate Kubernetes network policies, generate and list seccomp profiles, and create runtime policies and exceptions.

- **Base URL:** `https://api.armosec.io/api/v1`
- Tags: Network Policies, Seccomp, Runtime Policies, DevSecOps

### ARMO Registry Scanning API

Scan container image registries on demand or on a schedule. Issue a registry scan or set a scan scheduler (cron), and update or delete the registry scan cron job.

- **Base URL:** `https://api.armosec.io/api/v1`
- Tags: Registry, Image Scanning, Container Security

### ARMO Integrations API

Push ARMO findings into ticketing and collaboration tools. Configure Jira, look up projects/issue types/fields, create Jira issues from findings, and manage collaboration and notification configurations.

- **Base URL:** `https://api.armosec.io/api/v1`
- Tags: Integrations, Jira, Notifications

### ARMO Access Keys API

Programmatically manage the Agent Access Keys used to authenticate API calls. List, create, get by GUID, update, and delete access keys.

- **Base URL:** `https://api.armosec.io/api/v1`
- Tags: Authentication, Access Keys, Account

## Common Properties

- [Domain Security](security/armosec-domain-security.yml)
- [Authentication](authentication/armosec-authentication.yml)
- [GitHub Organization](https://github.com/armosec)
- [LinkedIn](https://www.linkedin.com/company/armosec)
- [Website](https://www.armosec.io/)
- [Documentation](https://hub.armosec.io/docs/armo-platform)
- [Plans](plans/armosec-plans-pricing.yml)
- [Rate Limits](rate-limits/armosec-rate-limits.yml)
- [Fin Ops](finops/armosec-finops.yml)
- [Blog](https://www.armosec.io/blog/)

## Open Source

ARMO's core scanning engine is the open-source **Kubescape** project ([github.com/kubescape/kubescape](https://github.com/kubescape/kubescape), a CNCF project) plus supporting components (eBPF node-agent sensor, storage, operator). ARMO Platform is the managed SaaS built on top, and is what the documented REST API belongs to.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
