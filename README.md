# Grafana

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

Grafana Labs builds the open and composable observability stack used by millions of engineers to visualize, query, alert on, and explore their metrics, logs, traces, and profiles. The flagship Grafana OSS dashboarding platform is paired with Grafana Loki (logs), Grafana Mimir (Prometheus-compatible metrics), Grafana Tempo (distributed traces), and Grafana Pyroscope (continuous profiling) — all under the LGTM stack. Grafana Cloud delivers the entire portfolio as a managed SaaS with a generous free tier, while Grafana Enterprise extends self-managed deployments with premium plugins, reporting, RBAC, LBAC, and caching. The ecosystem extends to Grafana k6 (load testing), Grafana Alloy (OpenTelemetry-native collector), Grafana Beyla (eBPF auto-instrumentation), Grafana Faro (frontend observability), Grafana OnCall (incident response), and Synthetic Monitoring. A canonical OpenAPI specification at public/api-merged.json powers the official Go client, the Terraform provider, the Grafana Operator, and a deep dashboards-as-code toolchain (Foundation SDK, Grafonnet, Grizzly, Scenes).

**Areas:** Observability · Monitoring · Dashboards · Logs · Metrics · Traces · Profiling · Alerting · Open Source · Grafana Labs

## Grafana on APIs.io

Everything profiled for Grafana is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/grafana-com/](https://apis.io/providers/grafana-com/)** — or go straight to one of the APIs or properties below.

### APIs (49)

- [Grafana Cloud API](https://apis.io/apis/grafana-com/grafana-cloud-api/) — Manage Grafana Cloud stacks (instances), plugins, data sources, regions, access policies, and tokens at `https://grafana.com/api`. Authenticated with Cloud…
- [Grafana Loki HTTP API](https://apis.io/apis/grafana-com/loki-http-api/) — Query and push logs to Grafana Loki. Endpoints include `/loki/api/v1/push` (log ingestion), `/loki/api/v1/query` and `/query_range` (LogQL),…
- [Grafana Mimir HTTP API](https://apis.io/apis/grafana-com/mimir-http-api/) — Horizontally scalable, multi-tenant, long-term Prometheus-compatible metrics storage. Exposes Prometheus remote-write at `/api/v1/push`, the full Prometheus…
- [Grafana Tempo HTTP API](https://apis.io/apis/grafana-com/tempo-http-api/) — High-volume, minimal-dependency distributed tracing backend. Supports OTLP ingestion, trace lookup by ID (`/api/traces/{traceID}`), TraceQL search…
- [Grafana Pyroscope HTTP API](https://apis.io/apis/grafana-com/pyroscope-http-api/) — Continuous profiling backend. Ingest pprof and Pyroscope-format CPU, memory, and lock profiles, query flame graphs and merge profiles, and run profile-based…
- [Grafana k6 Cloud API](https://apis.io/apis/grafana-com/k6-cloud-api/) — Programmatically trigger, list, and manage cloud-hosted k6 load tests, projects, organizations, test runs, thresholds, and results. Pairs with the…
- [Grafana OnCall API](https://apis.io/apis/grafana-com/oncall-api/) — Programmatic access to OnCall alert groups, integrations, escalation chains, schedules, on-call shifts, routes, slack channels, webhooks, and users. Powers…
- [Grafana Synthetic Monitoring API](https://apis.io/apis/grafana-com/synthetic-monitoring-api/) — Create and manage synthetic probes (HTTP, HTTPS, DNS, TCP, ICMP/ping, traceroute, multi-step scripted browser, gRPC) executed from Grafana Labs' global…
- [Grafana Access Control API](https://apis.io/apis/grafana-com/grafana-com-access-control-api/) — The API can be used to create, update, get and list roles, and create or remove built-in role assignments. To use the API, you would need to enable…
- [Grafana Admin API](https://apis.io/apis/grafana-com/grafana-com-admin-api/) — The Admin HTTP API does not currently work with an API Token. API Tokens are currently only linked to an organization and an organization role. They cannot…
- [Grafana Admin Ldap API](https://apis.io/apis/grafana-com/grafana-com-admin-ldap-api/) — The admin_ldap API from Grafana — 5 operation(s) for admin_ldap.
- [Grafana Admin Provisioning API](https://apis.io/apis/grafana-com/grafana-com-admin-provisioning-api/) — The admin_provisioning API from Grafana — 4 operation(s) for admin_provisioning.
- [Grafana Admin Users API](https://apis.io/apis/grafana-com/grafana-com-admin-users-api/) — The admin_users API from Grafana — 11 operation(s) for admin_users.
- [Grafana Annotations API](https://apis.io/apis/grafana-com/grafana-com-annotations-api/) — Grafana Annotations feature released in Grafana 4.6. Annotations are saved in the Grafana database (sqlite, mysql or postgres). Annotations can be…
- [Grafana Convert Prometheus API](https://apis.io/apis/grafana-com/grafana-com-convert-prometheus-api/) — The convert_prometheus API from Grafana — 6 operation(s) for convert_prometheus.
- [Grafana Correlations API](https://apis.io/apis/grafana-com/grafana-com-correlations-api/) — The correlations API from Grafana — 4 operation(s) for correlations.
- [Grafana Dashboard Public API](https://apis.io/apis/grafana-com/grafana-com-dashboard-public-api/) — The dashboard_public API from Grafana — 6 operation(s) for dashboard_public.
- [Grafana Dashboards API](https://apis.io/apis/grafana-com/grafana-com-dashboards-api/) — The dashboards API from Grafana — 20 operation(s) for dashboards.
- [Grafana Devices API](https://apis.io/apis/grafana-com/grafana-com-devices-api/) — The devices API from Grafana — 2 operation(s) for devices.
- [Grafana Enterprise API](https://apis.io/apis/grafana-com/grafana-com-enterprise-api/) — These are only available in Grafana Enterprise
- [Grafana Folders API](https://apis.io/apis/grafana-com/grafana-com-folders-api/) — Folders are identified by the identifier (id) and the unique identifier (uid). The identifier (id) of a folder is an auto-incrementing numeric value and is…
- [Grafana Health API](https://apis.io/apis/grafana-com/grafana-com-health-api/) — The health API from Grafana — 2 operation(s) for health.
- [Grafana Invites API](https://apis.io/apis/grafana-com/grafana-com-invites-api/) — The invites API from Grafana — 2 operation(s) for invites.
- [Grafana Library Elements API](https://apis.io/apis/grafana-com/grafana-com-library-elements-api/) — The identifier (ID) of a library element is an auto-incrementing numeric value that is unique per Grafana install. The unique identifier (UID) of a library…
- [Grafana Licensing API](https://apis.io/apis/grafana-com/grafana-com-licensing-api/) — Licensing is only available in Grafana Enterprise. Read more about Grafana Enterprise. If you are running Grafana Enterprise and have Fine-grained access…
- [Grafana Migrations API](https://apis.io/apis/grafana-com/grafana-com-migrations-api/) — The migrations API from Grafana — 10 operation(s) for migrations.
- [Grafana Org API](https://apis.io/apis/grafana-com/grafana-com-org-api/) — If you are running Grafana Enterprise and have Fine-grained access control enabled, for some endpoints you would need to have relevant permissions. Refer to…
- [Grafana Orgs API](https://apis.io/apis/grafana-com/grafana-com-orgs-api/) — The Admin Organizations HTTP API does not currently work with an API Token. API Tokens are currently only linked to an organization and an organization…
- [Grafana Permissions API](https://apis.io/apis/grafana-com/grafana-com-permissions-api/) — Permissions with `folderId=-1` are the default permissions for users with the Viewer and Editor roles. Permissions can be set for a user, a team or a role…
- [Grafana Playlists API](https://apis.io/apis/grafana-com/grafana-com-playlists-api/) — The playlists API from Grafana — 3 operation(s) for playlists.
- [Grafana Preferences API](https://apis.io/apis/grafana-com/grafana-com-preferences-api/) — The preferences API from Grafana — 3 operation(s) for preferences.
- [Grafana Provisioning API](https://apis.io/apis/grafana-com/grafana-com-provisioning-api/) — The provisioning API from Grafana — 17 operation(s) for provisioning.
- [Grafana Query History API](https://apis.io/apis/grafana-com/grafana-com-query-history-api/) — The identifier (ID) of a query in query history is an auto-incrementing numeric value that is unique per Grafana install. The unique identifier (UID) of a…
- [Grafana Quota API](https://apis.io/apis/grafana-com/grafana-com-quota-api/) — The quota API from Grafana — 6 operation(s) for quota.
- [Grafana Recording Rules API](https://apis.io/apis/grafana-com/grafana-com-recording-rules-api/) — The recording_rules API from Grafana — 4 operation(s) for recording_rules.
- [Grafana Reports API](https://apis.io/apis/grafana-com/grafana-com-reports-api/) — This API allows you to interact programmatically with the Reporting feature. Reporting is only available in Grafana Enterprise. Read more about Grafana…
- [Grafana SAML API](https://apis.io/apis/grafana-com/grafana-com-saml-api/) — The saml API from Grafana — 4 operation(s) for saml.
- [Grafana Search API](https://apis.io/apis/grafana-com/grafana-com-search-api/) — The search API from Grafana — 2 operation(s) for search.
- [Grafana Service Accounts API](https://apis.io/apis/grafana-com/grafana-com-service-accounts-api/) — If you are running Grafana Enterprise, for some endpoints you'll need to have specific permissions. Refer to [Role-based access control…
- [Grafana Signed In User API](https://apis.io/apis/grafana-com/grafana-com-signed-in-user-api/) — The signed_in_user API from Grafana — 10 operation(s) for signed_in_user.
- [Grafana Signing Keys API](https://apis.io/apis/grafana-com/grafana-com-signing-keys-api/) — The signing_keys API from Grafana — 1 operation(s) for signing_keys.
- [Grafana Snapshots API](https://apis.io/apis/grafana-com/grafana-com-snapshots-api/) — The snapshots API from Grafana — 5 operation(s) for snapshots.
- [Grafana SSO Settings API](https://apis.io/apis/grafana-com/grafana-com-sso-settings-api/) — The sso_settings API from Grafana — 2 operation(s) for sso_settings.
- [Grafana Sync Team Groups API](https://apis.io/apis/grafana-com/grafana-com-sync-team-groups-api/) — The sync_team_groups API from Grafana — 2 operation(s) for sync_team_groups.
- [Grafana Teams API](https://apis.io/apis/grafana-com/grafana-com-teams-api/) — This API can be used to create/update/delete Teams and to add/remove users to Teams. All actions require that the user has the Admin role for the organization.
- [Grafana User API](https://apis.io/apis/grafana-com/grafana-com-user-api/) — The user API from Grafana — 1 operation(s) for user.
- [Grafana Users API](https://apis.io/apis/grafana-com/grafana-com-users-api/) — The users API from Grafana — 6 operation(s) for users.
- [Grafana Versions API](https://apis.io/apis/grafana-com/grafana-com-versions-api/) — The versions API from Grafana — 3 operation(s) for versions.
- [Grafana Data Sources API](https://apis.io/apis/grafana-com/grafana-com-data-sources-api/) — If you are running Grafana Enterprise and have Fine-grained access control enabled, for some endpoints you would need to have relevant permissions. Refer to…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [grafana-com-mcp.yml](https://apis.io/servers/grafana-com/grafana-com-mcp-yml/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Grafana Com Agentic Access](https://apis.io/agentic-access/grafana-com/grafana-com-agentic-access/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Grafana API Rules](https://apis.io/rules/grafana-com/grafana-com-rules/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Grafana Com Authentication](https://apis.io/security/grafana-com/grafana-com-authentication/)
- [Grafana Com Domain Security](https://apis.io/security/grafana-com/grafana-com-domain-security/)
- [Grafana Com Trust Center](https://apis.io/security/grafana-com/grafana-com-trust-center/)
- [Grafana Com Vulnerability Disclosure](https://apis.io/security/grafana-com/grafana-com-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Grafana Com Plans Pricing](https://apis.io/plans/grafana-com/grafana-com-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Grafana Com Rate Limits](https://apis.io/rate-limits/grafana-com/grafana-com-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Grafana Com Finops](https://apis.io/finops/grafana-com/grafana-com-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.grafana.com/)
- [Documentation](https://grafana.com/docs/)
- [Getting started](https://grafana.com/docs/learning-paths/grafana-cloud-onboarding)
- [Pricing](https://grafana.com/pricing/)
- [Support](https://grafana.com/contact)
- [Changelog](https://grafana.com/docs/grafana/latest/whatsnew/)
- [Blog](https://grafana.com/blog/)
- [Compliance](https://trust.grafana.com/)
- [Trust centre](https://trust.grafana.com/)
- [Terms of service](https://grafana.com/legal/terms/)
- [Privacy policy](https://grafana.com/legal/privacy-policy/)
- [GitHub](https://github.com/grafana)
- [Status](https://status.grafana.com)

## API Evangelist rating

**Kin Score 64.3** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 47.3 |
| Contract governance | 22.0 |
| Operational transparency | 55.3 |
| Developer ergonomics | 75.6 |
| Access clarity | 76.3 |

**Agent readiness 31.1** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | mostly |

**Regulatory alignment 35.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/grafana-com/](https://apis.io/providers/grafana-com/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Grafana: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/grafana-com/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
