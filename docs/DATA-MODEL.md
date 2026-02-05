# Data Model

## Purpose
Define a minimal, shared schema that supports all industry packs.

## Core Entities
### Organization
- id
- name
- industry_pack
- settings

### User
- id
- org_id
- name
- email
- role

### Meeting
- id
- org_id
- title
- start_time
- end_time
- participants
- source (Teams/Zoom/Meet)

### Transcript
- id
- meeting_id
- storage_uri
- status

### Summary
- id
- meeting_id
- decisions
- action_items
- risks

### ActionItem
- id
- meeting_id
- owner_id
- due_date
- status

### Document
- id
- org_id
- title
- storage_uri
- sensitivity
- tags

### Workflow
- id
- org_id
- trigger
- rules

### Approval
- id
- workflow_id
- status
- approver_id

### AuditEvent
- id
- org_id
- actor_id
- action
- timestamp
- metadata

## Relationships
- Organization -> Users, Meetings, Documents, Workflows, AuditEvents
- Meeting -> Transcript, Summary, ActionItems
- Workflow -> Approvals

## Industry Extensions
- Stored as metadata on core entities or pack-specific templates
