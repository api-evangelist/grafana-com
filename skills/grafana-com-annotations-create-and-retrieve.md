---
name: grafana-com-annotations-create-and-retrieve
description: Create a new annotation and then retrieve it by its ID.
api: openapi/grafana-com-openapi.json
operations:
- postAnnotation
- getAnnotationByID
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/grafana-com-openapi.json ; every operationId checked against the contract
---

# grafana-com-annotations-create-and-retrieve

Create a new annotation and then retrieve it by its ID.

## Steps

1. 1. Use `postAnnotation` with the request body fields defined for creating an annotation (e.g., `time`, `timeEnd`, `text`, `tags`, `panelId`, `dashboardId`).
2. 2. Capture the `id` returned in the response.
3. 3. Use `getAnnotationByID` with the path parameter `annotation_id` set to the captured `id` to retrieve the created annotation.

## Rules

- Auth header: Include an `Authorization: Bearer <API_KEY>` header on all requests.
- Idempotency: `postAnnotation` is not idempotent; repeat calls will create duplicate annotations.
