# API Surface

## Purpose
Define the minimal API endpoints needed for integrations and UI.

## Meetings
- `POST /meetings/import`
- `GET /meetings/{id}`
- `GET /meetings/{id}/summary`
- `POST /meetings/{id}/actions`

## Documents
- `POST /documents/upload`
- `GET /documents/{id}`
- `POST /documents/{id}/tags`
- `POST /documents/{id}/share`

## Workflows
- `GET /workflows`
- `POST /workflows`
- `POST /workflows/{id}/activate`

## Approvals
- `GET /approvals`
- `POST /approvals/{id}/approve`
- `POST /approvals/{id}/reject`

## Dashboard
- `GET /dashboard/kpis`
- `GET /dashboard/alerts`

## Audit
- `GET /audit/events`
- `POST /audit/export`
