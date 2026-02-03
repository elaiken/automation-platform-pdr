# UI Wireframe Specs

## Purpose
Define the screen-level structure for demos and early builds. These specs are text-first wireframes to guide design and implementation.

## Global UI Principles
- Minimize clicks; surface decisions first.
- Keep compliance status visible but not overwhelming.
- Use consistent layout across industries with pack-specific widgets.

## Screen 1: Owner Dashboard
### Layout
- **Header**: Org name, date range selector, alerts icon
- **Left Nav**: Dashboard, Meetings, Documents, Workflows, Compliance, Settings
- **Main Grid** (2 columns)
  - **Top Row (Full Width)**: KPI Strip (Meeting volume, Action completion, Cycle time, Compliance risk)
  - **Left Column**: Action Health (overdue, due today, blocked), Workflow Bottlenecks
  - **Right Column**: Compliance Snapshot (retention exceptions, audit readiness), Industry Pack Highlights
  - **Bottom Row (Full Width)**: Trend chart (weekly actions completed vs overdue)

### Key Interactions
- Click KPI -> filtered list view
- Hover alerts -> quick remediation tips
- Export report -> CSV/PDF

## Screen 2: Meeting Recap
### Layout
- **Header**: Meeting title, date, participants, compliance status
- **Main Column**
  - Summary (paragraph)
  - Decisions (bullet list)
  - Action Items (table: owner, due date, status)
  - Risks / Notes
- **Right Rail**
  - Approvals (if required)
  - Related Docs
  - CRM / Task Sync status

### Key Interactions
- Approve / Request edits
- Assign action owner
- Link to doc or CRM record

## Screen 3: Document Intelligence
### Layout
- **Header**: Search bar, filters (type, owner, sensitivity)
- **Main List**: docs with tags and last updated
- **Right Preview**: extracted entities, summary, related meetings

### Key Interactions
- Apply tag, change sensitivity
- Share with internal/external

## Screen 4: Workflow Rules
### Layout
- **Rules list** (name, trigger, status)
- **Rule builder** (IF/THEN, approvals, routing)

### Key Interactions
- Test rule with sample data
- Activate / deactivate

## Industry Pack Variations
### Healthcare
- Compliance widget: HIPAA access checks
- KPI: care-task completion

### Financial Services
- Compliance widget: recordkeeping status
- KPI: supervision review SLAs

### Professional Services
- Compliance widget: privilege flags
- KPI: matter progress and utilization
