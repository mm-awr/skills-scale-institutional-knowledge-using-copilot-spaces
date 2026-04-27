# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

> See [Templates & Checklists](./octoacme-templates-and-checklists.md#risk-register-template) for a copy/paste Risk Register template including escalation paths.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Category (Technical / Schedule / Security / External)
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- **Owner** (named individual or role)
- Mitigation plan
- **Escalation path** (e.g., Team → PM → Product Lead → Sponsor)
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduce via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Risk Ownership
Each risk must have a named **Owner** who is accountable for driving the mitigation plan. Default ownership by risk type:
- **Technical risks** → Developer lead or SRE/DevOps
- **Security risks** → Security Lead
- **Schedule risks** → Project Manager
- **External/vendor risks** → Project Manager, escalated to Product Manager

## Escalation Paths
- Team-level → PM → Product Lead → Sponsor
- For security incidents, follow the security incident runbook and notify Security Lead on-call
- For production outages, SRE/DevOps leads the incident response and notifies PM and Stakeholders

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based) using the [Weekly Status Update template](./octoacme-templates-and-checklists.md#weekly-status-update-template)
- Use a single source of truth (project README or release doc) for status

## Stakeholder Comms Cadence

| Audience | Frequency | Format | Owner |
|---|---|---|---|
| Core delivery team | Daily standup | Verbal / async | Project Manager |
| Product Lead & PM | Weekly sync | Meeting + notes | Project Manager |
| Stakeholders | Weekly or milestone | Status update doc | Project Manager |
| Executive sponsor | Monthly or on escalation | Written summary | Product Manager |
| Operations | Pre-release | Readiness review | Project Manager |

## Communication Templates

**Weekly Status Update** — see [Templates & Checklists](./octoacme-templates-and-checklists.md#weekly-status-update-template)

**Incident Communication**
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled
