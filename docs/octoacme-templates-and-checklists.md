# OctoAcme Templates & Checklists

Reusable templates and checklists for consistent project execution. Copy the relevant section into your project documents and fill in the blanks.

> **See also:** [Roles & Personas](./octoacme-roles-and-personas.md) for role definitions referenced in the RACI template.

---

## RACI Matrix Template

Use this matrix to assign ownership for each key activity. Fill in **R** (Responsible), **A** (Accountable), **C** (Consulted), or **I** (Informed) for each role/activity combination. Leave a cell blank if the role is not involved.

| Activity / Deliverable | Project Manager | Product Manager | Developer | UX Designer | Security Lead | SRE/DevOps | Data Analyst | Operations | QA Lead | Stakeholder |
|---|---|---|---|---|---|---|---|---|---|---|
| Project One-pager | A | R | C | C | C | I | C | I | I | C |
| Backlog prioritization | C | A/R | C | C | I | I | C | I | C | C |
| UX research & prototyping | I | C | C | A/R | I | I | C | I | C | I |
| Security threat model | I | I | C | I | A/R | C | I | I | C | I |
| Test plan creation | C | C | C | C | C | C | I | C | A/R | I |
| Definition of Done sign-off | A | C | R | C | C | I | I | I | R | I |
| CI/CD pipeline setup | I | I | C | I | C | A/R | I | I | C | I |
| KPI / metrics definition | C | A | C | C | I | I | R | I | I | C |
| Deployment window decision | A | C | C | I | C | R | I | C | C | I |
| Release readiness sign-off | A | C | C | C | C | C | I | C | R | I |
| Stakeholder status update | R | C | I | I | I | I | C | I | I | A |
| Post-release incident response | I | I | R | I | C | A/R | I | C | C | I |
| Retrospective facilitation | A/R | C | C | C | I | C | I | C | C | I |

**Key:** R = Responsible · A = Accountable · C = Consulted · I = Informed

---

## Project Kickoff Agenda

**Meeting:** Project Kickoff  
**Duration:** 60–90 minutes  
**Facilitator:** Project Manager  
**Attendees:** Project Manager, Product Manager, Developers, UX Designer, QA Lead, Security Lead, SRE/DevOps, and relevant Stakeholders

### Agenda

| # | Topic | Owner | Time |
|---|---|---|---|
| 1 | Welcome & introductions | Project Manager | 5 min |
| 2 | Project background & problem statement | Product Manager | 10 min |
| 3 | Goals, success metrics, and Definition of Done | Product Manager | 10 min |
| 4 | Scope overview & what's out of scope | Product Manager | 10 min |
| 5 | Roles & responsibilities (RACI walkthrough) | Project Manager | 10 min |
| 6 | High-level timeline & milestones | Project Manager | 10 min |
| 7 | Known risks & dependencies | All | 10 min |
| 8 | Team norms & communication channels | Project Manager | 5 min |
| 9 | Open Q&A & next steps | All | 10 min |

### Pre-kickoff checklist
- [ ] Project One-pager shared at least 24 hours before the meeting
- [ ] Attendees confirmed and calendar invite sent
- [ ] Initial risk list drafted in the Risk Register
- [ ] Project board / repo created and linked in the invite

### Post-kickoff actions
- [ ] Kickoff notes and decisions documented and shared
- [ ] Backlog created with initial epics and stories
- [ ] RACI matrix populated and shared with all participants
- [ ] First sprint planning scheduled

---

## Weekly Status Update Template

**Project:** [Project Name]  
**Date:** [YYYY-MM-DD]  
**Author:** [Project Manager]  
**Distribution:** [Stakeholders, Product Manager, Delivery Team]

### Summary
[2–3 sentence executive summary of where the project stands.]

### Progress This Week
- [Completed item 1]
- [Completed item 2]
- [Completed item 3]

### Planned for Next Week
- [Planned item 1]
- [Planned item 2]
- [Planned item 3]

### Risks & Blockers

| Risk / Blocker | Impact | Owner | Mitigation / Status |
|---|---|---|---|
| [Description] | High / Med / Low | [Name / Role] | [Action being taken] |

### Metrics Snapshot
- Velocity / throughput: [value]
- Open bugs: [value]
- Test pass rate: [value]
- Key product metric: [value from Data Analyst dashboard]

### Decisions Needed
- [Decision 1 — who needs to decide, by when]
- [Decision 2 — who needs to decide, by when]

---

## Risk Register Template

Maintain one row per identified risk. Review at each weekly sync and update Status accordingly.

| ID | Description | Category | Impact | Likelihood | Risk Score | Owner | Mitigation Plan | Escalation Path | Status | Last Updated |
|---|---|---|---|---|---|---|---|---|---|---|
| R-001 | [Risk description] | Technical / Schedule / Security / External | H/M/L | H/M/L | H×H=H | [Role] | [Mitigation steps] | PM → Product Lead → Sponsor | Open | [Date] |
| R-002 | | | | | | | | | | |

**Risk Score guide:**
- High × High = Critical — immediate mitigation required
- High × Med or Med × High = High — mitigate this sprint
- Med × Med or below = Medium/Low — monitor and review weekly

**Categories:**
- **Technical:** architecture, integration, or implementation uncertainty
- **Schedule:** timeline pressure, dependency slippage, resource constraints
- **Security:** vulnerability, compliance, or data exposure risk
- **External:** third-party, vendor, or regulatory dependency

---

## Release Readiness Checklist

Complete this checklist before any production release. All items must be checked or explicitly waived with justification.

### Pre-Release

#### Code & Quality
- [ ] All acceptance criteria met and verified by QA Lead
- [ ] Definition of Done signed off for all included items
- [ ] All PRs merged; no open PRs blocking this release
- [ ] CI pipeline passes (tests, linting, security scans)
- [ ] No unresolved P0/P1 bugs in scope of this release
- [ ] Security Lead sign-off (threat model reviewed, no critical findings open)

#### Documentation & Communication
- [ ] Release notes drafted and reviewed
- [ ] Stakeholders notified of release date and scope
- [ ] Operations support playbook / runbook updated
- [ ] Customer-facing documentation updated (if applicable)

#### Infrastructure & Deployment
- [ ] Deployment window confirmed with SRE/DevOps and Operations
- [ ] Rollback plan documented and tested (or waived with reason)
- [ ] Feature flags configured correctly (if applicable)
- [ ] Monitoring alerts and dashboards validated
- [ ] Staging deployment completed and verified

### Release Execution

- [ ] Production deployment initiated by SRE/DevOps
- [ ] Post-deploy smoke tests passed
- [ ] Error rate, latency, and key metrics within normal bounds
- [ ] Release announcement sent to stakeholders and support channels

### Post-Release Verification (within 24–48 hours)

- [ ] Key product metrics trending as expected (Data Analyst review)
- [ ] Support ticket volume reviewed by Operations
- [ ] No unexpected incidents or rollbacks required
- [ ] Retrospective or release debrief scheduled (if major release)

**Release Readiness Owner:** [Project Manager]  
**QA Sign-off:** [QA Lead Name / Date]  
**Security Sign-off:** [Security Lead Name / Date]  
**SRE/DevOps Sign-off:** [SRE/DevOps Name / Date]

---

## Definition of Done (DoD) Template

Adapt this baseline DoD to your project. All items must be met before a story or feature is considered Done.

### Standard Definition of Done

- [ ] Code implemented and peer-reviewed (at least one approval)
- [ ] All acceptance criteria met as verified by the author and QA
- [ ] Unit tests written and passing (coverage maintained or improved)
- [ ] Integration / end-to-end tests updated where applicable
- [ ] Security review completed for features touching auth, data, or APIs
- [ ] Accessibility standards met (WCAG 2.1 AA or team-agreed level)
- [ ] Documentation updated (README, API docs, runbooks as appropriate)
- [ ] Feature flag or rollout strategy confirmed with SRE/DevOps
- [ ] QA Lead sign-off recorded in the issue or PR

### Optional / Project-Specific Items
- [ ] Data Analyst event tracking implemented and verified
- [ ] UX Designer usability review passed
- [ ] Operations runbook / support guide updated
- [ ] Stakeholder demo or sign-off completed
