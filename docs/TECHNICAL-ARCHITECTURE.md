# Technical Architecture

## Purpose
Define the system-level structure for the shared platform and industry packs.

## High-Level Services
- **Ingestion Service**: meeting connectors, document sources
- **Processing Service**: transcription, summarization, extraction
- **Workflow Service**: rules engine, approvals, routing
- **Knowledge Service**: search, embeddings, Q&A with citations
- **Policy Service**: retention, access control, audit trails
- **Integration Service**: CRM, task tools, email
- **Dashboard Service**: analytics, KPIs, reporting

## Data Stores
- **Relational DB**: users, orgs, actions, workflows
- **Object Storage**: documents, transcripts
- **Search Index**: semantic + keyword search
- **Audit Log Store**: immutable event log

## Core Entities
- Organization, User, Role
- Meeting, Transcript, Summary
- ActionItem, Workflow, Approval
- Document, Tag, Sensitivity
- AuditEvent, RetentionPolicy

## Integration Pattern
- Webhooks for event triggers
- Scheduled sync for slow systems
- OAuth for user-based access

## Security
- Encryption in transit and at rest
- Role-based access control
- Per-industry retention rules
- Audit log immutability

## Industry Packs (Configuration Layer)
- Templates and rules stored as configuration
- No core code forks
- Versioned pack releases

## Deployment Targets
- Cloud-first with optional private deployment
- Separation of tenant data at all layers
