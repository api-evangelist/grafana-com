---
name: grafana-com-create-folder
description: Create a new folder, retrieve it, optionally update its details, and then delete it.
api: openapi/grafana-com-openapi.json
operations:
- createFolder
- getFolderByUID
- updateFolder
- deleteFolder
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/grafana-com-openapi.json ; every operationId checked against the contract
---

# grafana-com-create-folder

Create a new folder, retrieve it, optionally update its details, and then delete it.

## Steps

1. 1. Use `createFolder` with body fields `title`, `uid` (optional) and header `Content-Type: application/json`.
2. 2. Use `getFolderByUID` with path parameter `folder_uid` returned from step 1.
3. 3. Use `updateFolder` with path parameter `folder_uid` and body fields to modify, header `Content-Type: application/json`.
4. 4. Use `deleteFolder` with path parameter `folder_uid`.

## Rules

- Authentication: Include an `Authorization` header with a valid API token.
- Rate limiting: No rate limit is defined; on exhaustion the API returns no specific HTTP status.
