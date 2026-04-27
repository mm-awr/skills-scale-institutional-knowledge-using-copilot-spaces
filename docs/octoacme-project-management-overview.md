# OctoAcme Project Management Overview

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Lead.
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles
- **Project Manager (PM):** coordinates delivery, schedules, risk, communications.
- **Product Manager (PdM):** defines outcomes, prioritizes backlog, and measures success.
- **Developers:** implement features, collaborate on design and testability.
- **UX Designer:** leads user research, design specs, and usability validation.
- **Security Lead:** owns threat modeling, secure-development guidance, and security sign-off.
- **SRE/DevOps:** manages CI/CD, reliability, and incident response.
- **Data Analyst:** defines KPIs, builds dashboards, and supports data-driven decisions.
- **Operations:** handles post-release support readiness, runbooks, and customer impact.
- **QA Lead:** coordinates test strategy, acceptance sign-off, and Definition of Done.
- **Stakeholders:** provide requirements, approvals, and business direction.

> See [Roles & Personas](./octoacme-roles-and-personas.md) for detailed responsibilities and cross-role interactions, and [Templates & Checklists](./octoacme-templates-and-checklists.md) for a pre-populated RACI matrix template.

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- Risk Register
- Retrospective notes and action items

## Lifecycle (high-level)
1. Initiation: problem statement, stakeholders, high-level timeline.
2. Planning: scope, resources, milestones, dependencies.
3. Execution: build, test, review, iterate.
4. Release: deploy, verify, announce.
5. Close & Retrospective: capture learnings and next steps.

## Communication Cadence
- Weekly sync between PM + PdM
- Twice-weekly standups for delivery team (or as agreed)
- Monthly stakeholder updates
- Ad-hoc escalations as needed

## How to use these docs
- Keep the Project Charter updated in the project repo.
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context.
- Use [Templates & Checklists](./octoacme-templates-and-checklists.md) to copy/paste reusable RACI matrices, kickoff agendas, status updates, risk registers, and release readiness checklists.
- Review [Roles & Personas](./octoacme-roles-and-personas.md) during project kickoff to agree on who fills each role for your project.
