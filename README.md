# ARMO

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

ARMO is the cloud-native and Kubernetes security company behind the leading open-source project Kubescape. ARMO Platform is a runtime-driven CNAPP that unifies Kubernetes Security Posture Management (KSPM), vulnerability and image scanning, compliance frameworks, network and seccomp policy generation, and runtime Cloud Application Detection and Response (CADR) - correlating runtime behavior with posture and vulnerabilities to cut alert noise. ARMO exposes a documented REST API over HTTPS (base https://api.armosec.io/api/v1 in the EU region and https://api.us.armosec.io/api/v1 in the US region), authenticated with an account access key sent in the X-API-KEY header. The API covers clusters, workloads, vulnerabilities, posture and compliance, security risks, runtime incidents, attack chains, network and runtime policies, registry scanning, and integrations. API access is available to platform customers who have generated an Agent Access Key; the endpoints below are documented but the data returned requires a connected account and clusters.

**Areas:** Kubernetes Security · Cloud Native Security · CNAPP · DevSecOps · KSPM · Vulnerability Management · Compliance · Runtime Security · CADR · Kubescape · Container Security

## ARMO on APIs.io

Everything profiled for ARMO is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/armosec/](https://apis.io/providers/armosec/)** — or go straight to one of the APIs or properties below.

### APIs (8)

- [ARMO Access Keys API](https://apis.io/apis/armosec/armosec-access-keys-api/) — Account API access key management.
- [ARMO Clusters API](https://apis.io/apis/armosec/armosec-clusters-api/) — Connected clusters and workloads.
- [ARMO Integrations API](https://apis.io/apis/armosec/armosec-integrations-api/) — Jira and collaboration/notification integrations.
- [ARMO Posture API](https://apis.io/apis/armosec/armosec-posture-api/) — KSPM posture and compliance framework results.
- [ARMO Registry API](https://apis.io/apis/armosec/armosec-registry-api/) — Container registry scanning.
- [ARMO Runtime API](https://apis.io/apis/armosec/armosec-runtime-api/) — Runtime incidents (CADR), network and runtime policies.
- [ARMO Security Risks API](https://apis.io/apis/armosec/armosec-security-risks-api/) — Correlated security risks and attack chains.
- [ARMO Vulnerabilities API](https://apis.io/apis/armosec/armosec-vulnerabilities-api/) — Image and workload vulnerability scanning and results.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [armosec](https://apis.io/servers/armosec/armosec/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Armosec Agentic Access](https://apis.io/agentic-access/armosec/armosec-agentic-access/)

#### Collections (9)

Postman and Open Collection request collections.

- [ARMO Platform API](https://apis.io/collections/armosec/open-armosec/)
- [ARMO Platform Access Keys API](https://apis.io/collections/armosec/open-armosec-access-keys-api/)
- [ARMO Platform Access Keys Clusters API](https://apis.io/collections/armosec/open-armosec-clusters-api/)
- [ARMO Platform Access Keys Integrations API](https://apis.io/collections/armosec/open-armosec-integrations-api/)
- [ARMO Platform Access Keys Posture API](https://apis.io/collections/armosec/open-armosec-posture-api/)
- [ARMO Platform Access Keys Registry API](https://apis.io/collections/armosec/open-armosec-registry-api/)
- [ARMO Platform Access Keys Runtime API](https://apis.io/collections/armosec/open-armosec-runtime-api/)
- [ARMO Platform Access Keys Security Risks API](https://apis.io/collections/armosec/open-armosec-security-risks-api/)
- [ARMO Platform Access Keys Vulnerabilities API](https://apis.io/collections/armosec/open-armosec-vulnerabilities-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Armosec Authentication](https://apis.io/security/armosec/armosec-authentication/)
- [Armosec Domain Security](https://apis.io/security/armosec/armosec-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Armosec Plans Pricing](https://apis.io/plans/armosec/armosec-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Armosec Rate Limits](https://apis.io/rate-limits/armosec/armosec-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Armosec Finops](https://apis.io/finops/armosec/armosec-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.armosec.io/)
- [Documentation](https://hub.armosec.io/docs/armo-platform)
- [Blog](https://www.armosec.io/blog/)
- [GitHub](https://github.com/armosec)

## API Evangelist rating

**Kin Score 25.2** — emerging · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 68.3 |
| Contract quality | 44.4 |
| Contract governance | 0.0 |
| Operational transparency | 10.5 |
| Developer ergonomics | 27.4 |
| Access clarity | 7.9 |

**Agent readiness 28.5** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | mostly |

**Regulatory alignment 11.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/armosec/](https://apis.io/providers/armosec/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for ARMO: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/armosec/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
