# ARMO (armosec)

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
