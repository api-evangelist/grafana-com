# Grafana (grafana-com)

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

Grafana Labs builds the open and composable observability stack used by millions of engineers to visualize, query, alert on, and explore their metrics, logs, traces, and profiles. The flagship Grafana OSS dashboarding platform is paired with Grafana Loki (logs), Grafana Mimir (Prometheus-compatible metrics), Grafana Tempo (distributed traces), and Grafana Pyroscope (continuous profiling) — all under the LGTM stack. Grafana Cloud delivers the entire portfolio as a managed SaaS with a generous free tier, while Grafana Enterprise extends self-managed deployments with premium plugins, reporting, RBAC, LBAC, and caching. The ecosystem extends to Grafana k6 (load testing), Grafana Alloy (OpenTelemetry-native collector), Grafana Beyla (eBPF auto-instrumentation), Grafana Faro (frontend observability), Grafana OnCall (incident response), and Synthetic Monitoring. A canonical OpenAPI specification at `public/api-merged.json` powers the official Go client, the Terraform provider, the Grafana Operator, and a deep dashboards-as-code toolchain (Foundation SDK, Grafonnet, Grizzly, Scenes).

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/grafana-com/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Observability, Monitoring, Dashboards, Logs, Metrics, Traces, Profiling, Alerting, Open Source, Grafana Labs

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## The LGTM Stack at a Glance

| Product | Telemetry | Query Language | Repo |
|---|---|---|---|
| **Grafana** | Visualization | — | [grafana/grafana](https://github.com/grafana/grafana) |
| **Loki** | Logs | LogQL | [grafana/loki](https://github.com/grafana/loki) |
| **Mimir** | Metrics | PromQL | [grafana/mimir](https://github.com/grafana/mimir) |
| **Tempo** | Traces | TraceQL | [grafana/tempo](https://github.com/grafana/tempo) |
| **Pyroscope** | Profiles | Pyroscope query / pprof | [grafana/pyroscope](https://github.com/grafana/pyroscope) |
| **Alloy** | OTel Collector | — | [grafana/alloy](https://github.com/grafana/alloy) |
| **k6** | Load Testing | JavaScript | [grafana/k6](https://github.com/grafana/k6) |
| **Beyla** | eBPF auto-instrumentation | — | [grafana/beyla](https://github.com/grafana/beyla) |
| **Faro** | Frontend observability | — | [grafana/faro-web-sdk](https://github.com/grafana/faro-web-sdk) |
| **OnCall** | Incident response | — | [grafana/oncall](https://github.com/grafana/oncall) |

## APIs

### Grafana HTTP API
The full Grafana HTTP API surface for self-managed Grafana and Grafana Enterprise, with a canonical OpenAPI 2.0 specification at `public/api-merged.json` in the grafana/grafana repository.

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/](https://grafana.com/docs/grafana/latest/developers/http_api/)

- [Documentation](https://grafana.com/docs/grafana/latest/developers/http_api/)
- [Canonical OpenAPI Specification](https://github.com/grafana/grafana/blob/main/public/api-merged.json)
- [Authentication](https://grafana.com/docs/grafana/latest/developers/http_api/authentication/)

### Grafana Dashboard API
Create, read, update, delete, search, version, and permission dashboards via the Kubernetes-style `dashboard.grafana.app/v1` and legacy `/api/dashboards/` endpoints.

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/dashboard/](https://grafana.com/docs/grafana/latest/developers/http_api/dashboard/)

- [Documentation](https://grafana.com/docs/grafana/latest/developers/http_api/dashboard/)
- [Dashboard Versions](https://grafana.com/docs/grafana/latest/developers/http_api/dashboard_versions/)
- [Dashboard Permissions](https://grafana.com/docs/grafana/latest/developers/http_api/dashboard_permissions/)
- [Shared (Public) Dashboards](https://grafana.com/docs/grafana/latest/developers/http_api/dashboard_public/)

### Grafana Folder and Search API
Manage folders, cross-folder dashboard search, and folder-level permissions — the primary organizational unit for dashboards.

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/folder/](https://grafana.com/docs/grafana/latest/developers/http_api/folder/)

- [Documentation](https://grafana.com/docs/grafana/latest/developers/http_api/folder/)
- [Folder/Dashboard Search](https://grafana.com/docs/grafana/latest/developers/http_api/folder_dashboard_search/)
- [Folder Permissions](https://grafana.com/docs/grafana/latest/developers/http_api/folder_permissions/)

### Grafana Data Source API
Programmatically register and manage data sources (Prometheus, Loki, Tempo, Mimir, Pyroscope, plus 150+ more) with per-data-source permissions and label-based access control (LBAC) rules.

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/data_source/](https://grafana.com/docs/grafana/latest/developers/http_api/data_source/)

- [Documentation](https://grafana.com/docs/grafana/latest/developers/http_api/data_source/)
- [Data Source Permissions](https://grafana.com/docs/grafana/latest/developers/http_api/datasource_permissions/)
- [Data Source LBAC Rules](https://grafana.com/docs/grafana/latest/developers/http_api/datasource_lbac_rules/)

### Grafana Alerting Provisioning API
Provision alert rules, contact points, mute timings, notification policies, and templates for GitOps-style alert-as-code.

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/alerting_provisioning/](https://grafana.com/docs/grafana/latest/developers/http_api/alerting_provisioning/)

### Grafana Annotations API
Create, read, update, and delete annotations marking events on time-series dashboards.

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/annotations/](https://grafana.com/docs/grafana/latest/developers/http_api/annotations/)

### Grafana Organization and Users API
Manage organizations, users, teams, external team sync, and user/org preferences.

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/org/](https://grafana.com/docs/grafana/latest/developers/http_api/org/)

- [Users](https://grafana.com/docs/grafana/latest/developers/http_api/user/)
- [Teams](https://grafana.com/docs/grafana/latest/developers/http_api/team/)
- [Team Sync](https://grafana.com/docs/grafana/latest/developers/http_api/team_sync/)
- [Preferences](https://grafana.com/docs/grafana/latest/developers/http_api/preferences/)

### Grafana Access Control (RBAC) API
Fine-grained RBAC, custom roles, permission grants, service accounts, service account tokens, and SSO settings (SAML, OAuth, LDAP).

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/access_control/](https://grafana.com/docs/grafana/latest/developers/http_api/access_control/)

- [Service Accounts](https://grafana.com/docs/grafana/latest/developers/http_api/serviceaccount/)
- [SSO Settings](https://grafana.com/docs/grafana/latest/developers/http_api/sso-settings/)

### Grafana Admin API
Server-wide administration plus Grafana Enterprise extensions for licensing, scheduled reporting, and query/resource caching.

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/admin/](https://grafana.com/docs/grafana/latest/developers/http_api/admin/)

- [Enterprise Licensing](https://grafana.com/docs/grafana/latest/developers/http_api/licensing/)
- [Reporting (Enterprise)](https://grafana.com/docs/grafana/latest/developers/http_api/reporting/)
- [Query and Resource Caching (Enterprise)](https://grafana.com/docs/grafana/latest/developers/http_api/query_and_resource_caching/)

### Grafana Library Elements API
Reusable library panels and variables that propagate updates to every dashboard that references them.

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/library_element/](https://grafana.com/docs/grafana/latest/developers/http_api/library_element/)

### Grafana Correlations API
Define click-through pivots between data sources to connect metrics, logs, traces, and profiles in Explore and dashboards.

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/correlations/](https://grafana.com/docs/grafana/latest/developers/http_api/correlations/)

### Grafana Snapshot, Short URL, and Query History API
Share dashboard snapshots, generate short URLs for long Explore queries, and read/write Explore query history.

**Human URL:** [https://grafana.com/docs/grafana/latest/developers/http_api/snapshot/](https://grafana.com/docs/grafana/latest/developers/http_api/snapshot/)

- [Short URLs](https://grafana.com/docs/grafana/latest/developers/http_api/short_url/)
- [Query History](https://grafana.com/docs/grafana/latest/developers/http_api/query_history/)

### Grafana Cloud API
Manage Grafana Cloud stacks, plugins, regions, access policies, and tokens at `https://grafana.com/api`. The recommended automation surface for provisioning Grafana Cloud environments and Terraform workflows.

**Human URL:** [https://grafana.com/docs/grafana-cloud/developer-resources/api-reference/cloud-api/](https://grafana.com/docs/grafana-cloud/developer-resources/api-reference/cloud-api/)

- [Access Policies and Tokens](https://grafana.com/docs/grafana-cloud/account-management/authentication-and-permissions/access-policies/)

### Grafana Loki HTTP API
Push and query logs with LogQL. Endpoints include `/loki/api/v1/push`, `/query`, `/query_range`, `/labels`, `/series`, and `/tail` (websocket streaming).

**Human URL:** [https://grafana.com/docs/loki/latest/reference/loki-http-api/](https://grafana.com/docs/loki/latest/reference/loki-http-api/)

### Grafana Mimir HTTP API
Prometheus remote-write metrics ingestion plus the full Prometheus query API, ruler, alertmanager, and per-tenant admin endpoints.

**Human URL:** [https://grafana.com/docs/mimir/latest/references/http-api/](https://grafana.com/docs/mimir/latest/references/http-api/)

### Grafana Tempo HTTP API
OTLP trace ingestion, trace lookup by ID, TraceQL search, and span-derived metrics over object storage.

**Human URL:** [https://grafana.com/docs/tempo/latest/api_docs/](https://grafana.com/docs/tempo/latest/api_docs/)

### Grafana Pyroscope HTTP API
Continuous profiling ingest (pprof and Pyroscope formats), flame-graph queries, and merge/diff operations.

**Human URL:** [https://grafana.com/docs/pyroscope/latest/configure-server/about-server-api/](https://grafana.com/docs/pyroscope/latest/configure-server/about-server-api/)

### Grafana k6 Cloud API
Trigger and manage cloud-hosted k6 load tests, projects, organizations, thresholds, and results.

**Human URL:** [https://grafana.com/docs/grafana-cloud/testing/k6/reference/cloud-rest-api/](https://grafana.com/docs/grafana-cloud/testing/k6/reference/cloud-rest-api/)

### Grafana OnCall API
Programmatic access to alert groups, integrations, escalation chains, schedules, on-call shifts, routes, and webhooks.

**Human URL:** [https://grafana.com/docs/oncall/latest/oncall-api-reference/](https://grafana.com/docs/oncall/latest/oncall-api-reference/)

### Grafana Synthetic Monitoring API
Create synthetic probes (HTTP/HTTPS, DNS, TCP, ICMP, traceroute, scripted browser, gRPC) executed from a global probe network.

**Human URL:** [https://grafana.com/docs/grafana-cloud/monitor-public-endpoints/](https://grafana.com/docs/grafana-cloud/monitor-public-endpoints/)

## Common Properties

- [Portal — grafana.com](https://grafana.com)
- [Documentation — Grafana Docs](https://grafana.com/docs/)
- [Documentation — Grafana OSS Docs](https://grafana.com/docs/grafana/latest/)
- [Documentation — Grafana Cloud Docs](https://grafana.com/docs/grafana-cloud/)
- [Documentation — HTTP API Reference](https://grafana.com/docs/grafana/latest/developers/http_api/)
- [OpenAPI — Canonical Grafana Spec](https://github.com/grafana/grafana/blob/main/public/api-merged.json)
- [Documentation — Developer Resources](https://grafana.com/docs/grafana/latest/developers/)
- [Authentication — HTTP API](https://grafana.com/docs/grafana/latest/developers/http_api/authentication/)
- [Authentication — Grafana Cloud Access Policies](https://grafana.com/docs/grafana-cloud/account-management/authentication-and-permissions/access-policies/)
- [GitHubOrganization](https://github.com/grafana)
- [SourceCode — grafana/grafana](https://github.com/grafana/grafana)
- [Documentation — Community Dashboards Library](https://grafana.com/grafana/dashboards/)
- [Documentation — Plugin Catalog](https://grafana.com/grafana/plugins/)
- [Documentation — Plugin Developer Docs](https://grafana.com/docs/plugins/)
- [Tool — Plugin Tools (create-plugin)](https://grafana.com/developers/plugin-tools/)
- [Documentation — Scenes](https://grafana.com/developers/scenes)
- [Documentation — Saga Design System](https://grafana.com/developers/saga-design-system/)
- [SDK — Grafana Foundation SDK](https://github.com/grafana/grafana-foundation-sdk)
- [SDK — Grafana OpenAPI Client (Go)](https://github.com/grafana/grafana-openapi-client-go)
- [SDK — Grafana API Go Client (legacy)](https://github.com/grafana/grafana-api-golang-client)
- [SDK — Grafana Plugin SDK (Go)](https://github.com/grafana/grafana-plugin-sdk-go)
- [SDK — Grafonnet](https://github.com/grafana/grafonnet)
- [SDK — Faro Web SDK](https://github.com/grafana/faro-web-sdk)
- [Tool — Terraform Provider for Grafana](https://github.com/grafana/terraform-provider-grafana)
- [Tool — Grafana Operator (Kubernetes)](https://github.com/grafana/grafana-operator)
- [Tool — Grafana Helm Charts](https://github.com/grafana/helm-charts)
- [Tool — Grafana Image Renderer](https://github.com/grafana/grafana-image-renderer)
- [Tool — Grizzly](https://github.com/grafana/grizzly)
- [SourceCode — Loki](https://github.com/grafana/loki)
- [SourceCode — Mimir](https://github.com/grafana/mimir)
- [SourceCode — Tempo](https://github.com/grafana/tempo)
- [SourceCode — Pyroscope](https://github.com/grafana/pyroscope)
- [SourceCode — k6](https://github.com/grafana/k6)
- [SourceCode — Alloy](https://github.com/grafana/alloy)
- [SourceCode — Beyla](https://github.com/grafana/beyla)
- [SourceCode — OnCall](https://github.com/grafana/oncall)
- [SourceCode — Synthetic Monitoring Agent](https://github.com/grafana/synthetic-monitoring-agent)
- [Pricing — Grafana Cloud](https://grafana.com/pricing/)
- [RateLimits — Data Source Rate Limiting](https://grafana.com/docs/grafana/latest/setup-grafana/configure-grafana/configure-rate-limit-data-source/)
- [StatusPage](https://status.grafana.com)
- [Blog](https://grafana.com/blog/)
- [Blog — Engineering](https://grafana.com/blog/categories/engineering/)
- [Events — GrafanaCON](https://grafana.com/events/grafanacon/)
- [TermsOfService](https://grafana.com/legal/terms/)
- [PrivacyPolicy](https://grafana.com/legal/privacy-policy/)
- [TrustCenter](https://trust.grafana.com/)
- [SignUp](https://grafana.com/auth/sign-up)
- [Portal — Grafana Cloud](https://grafana.com/products/cloud/)
- [Portal — Grafana Enterprise](https://grafana.com/products/enterprise/)
- [Sandbox — Grafana Play](https://grafana.com/play/)
- [Forum — Community](https://community.grafana.com/)
- [Forum — GitHub Discussions](https://github.com/grafana/grafana/discussions)
- [Training — Tutorials](https://grafana.com/tutorials/)
- [Training — Grafana University](https://university.grafana.com/)
- [Versioning — Release Life Cycle](https://grafana.com/docs/release-life-cycle/)
- [ChangeLog — What's New](https://grafana.com/docs/grafana/latest/whatsnew/)
- [LinkedIn](https://www.linkedin.com/company/grafana-labs)
- [Twitter](https://twitter.com/grafana)
- [YouTube](https://www.youtube.com/c/Grafana)
- [Mastodon](https://fosstodon.org/@grafana)

## Commercial Artifacts

- [Plans / Pricing](plans/grafana-com-plans-pricing.yml)
- [Rate Limits](rate-limits/grafana-com-rate-limits.yml)
- [FinOps Definition](finops/grafana-com-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
