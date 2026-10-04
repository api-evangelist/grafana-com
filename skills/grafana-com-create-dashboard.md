---
name: grafana-com-create-dashboard
description: Create a new dashboard and retrieve it by its UID.
api: openapi/grafana-com-openapi.json
operations:
- postDashboard
- getDashboardByUID
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/grafana-com-openapi.json ; every operationId checked against the contract
---

# grafana-com-create-dashboard

Create a new dashboard and retrieve it by its UID.

## Steps

1. 1. Use `postDashboard` with the dashboard JSON payload in the request body.
2. 2. Use `getDashboardByUID` with the `uid` returned from the previous step as a path parameter.

## Rules

- Auth header: Include an `Authorization: Bearer <API_KEY>` header on each request.
- Idempotency: `postDashboard` is upsert; sending the same payload with the same UID will update the existing dashboard.
