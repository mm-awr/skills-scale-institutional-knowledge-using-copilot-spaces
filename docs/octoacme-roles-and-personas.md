# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

> **See also:** [Templates & Checklists](./octoacme-templates-and-checklists.md) for a RACI matrix template and other reusable artifacts that reference these roles.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

### Interactions with Other Roles
- Collaborate with **UX Designer** on implementation of design specs and prototypes
- Receive acceptance criteria from **Product Manager** and **QA Lead**
- Coordinate with **SRE/DevOps** on pipeline reliability, deployment steps, and incident response
- Consult **Security Lead** during design reviews and for threat-model guidance
- Support **Data Analyst** with event tracking and instrumentation

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

### Interactions with Other Roles
- Partner with **UX Designer** on user research, design direction, and feature validation
- Work with **Data Analyst** to define KPIs and review feature adoption metrics
- Coordinate with **Project Manager** on scope, timelines, and risks
- Engage **Stakeholders** for requirements sign-off and milestone reviews
- Align with **QA Lead** on acceptance criteria and Definition of Done

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

### Interactions with Other Roles
- Coordinate with **Product Manager** on scope changes and backlog priority
- Escalate risks identified by **Security Lead** or **SRE/DevOps** to Stakeholders
- Engage **Operations** early on rollout plans and support handoff
- Work with **QA Lead** to track testing progress and Definition of Done sign-off
- Keep **Stakeholders** informed via regular status updates and milestone reviews

---

## UX Designer

### Role Summary
UX Designers ensure usability and user advocacy throughout project discovery, design, and validation phases. They bridge the gap between user needs and technical implementation.

### Responsibilities
- Lead or facilitate user research and usability testing
- Create wireframes, mockups, and interactive prototypes
- Define UX acceptance criteria for features
- Review implemented features for usability before QA sign-off
- Maintain a design system or style guide for consistency

### Goals
- Deliver intuitive, accessible, and high-quality user experiences
- Reduce rework by validating designs early with real users
- Align visual and interaction design with product goals

### Typical Communication
- Design reviews and prototype demos in sprint reviews
- Async feedback on PRs with UI changes
- Design handoff notes in the project wiki or design tool

### Interactions with Other Roles
- Co-create feature specs with **Product Manager** based on user research
- Hand off design assets and specs to **Developers** for implementation
- Collaborate with **QA Lead** to define usability acceptance criteria
- Incorporate **Stakeholder** feedback into design iterations
- Consult **Data Analyst** for insights on user behavior and feature adoption

---

## Security Lead

### Role Summary
Security Leads own security risk management, support secure development practices, and validate that releases address threat models and comply with data/privacy requirements.

### Responsibilities
- Assess projects for security risks and produce threat models
- Review designs and implementations for vulnerabilities
- Advise on data handling, privacy compliance, and secure coding standards
- Define and maintain the security incident runbook
- Validate security sign-off before release

### Goals
- Reduce the attack surface and ensure secure-by-default practices
- Ensure compliance with organizational and regulatory requirements
- Minimize mean time to detect and respond to security incidents

### Typical Communication
- Security review comments on PRs and design docs
- Participation in kickoff and planning meetings for high-risk features
- Incident notifications and post-incident reports

### Interactions with Other Roles
- Consult with **Developers** during design and code review phases
- Escalate security risks to **Project Manager** and **Stakeholders**
- Coordinate with **SRE/DevOps** on security scanning in CI/CD and incident response
- Advise **Product Manager** on data/privacy constraints that affect feature scope
- Partner with **QA Lead** to ensure security test cases are included in test plans

---

## SRE/DevOps

### Role Summary
SREs and DevOps engineers ensure system reliability, smooth deployments, and automated operations. They own the CI/CD pipeline and lead incident management.

### Responsibilities
- Design, maintain, and improve CI/CD pipelines
- Monitor system uptime, latency, and error rates
- Automate rollback procedures and infrastructure as code
- Lead blameless incident retrospectives and drive reliability improvements
- Define and enforce SLOs/SLAs

### Goals
- Maximize system availability and deployment frequency
- Reduce mean time to recovery (MTTR)
- Ensure infrastructure changes are auditable and reproducible

### Typical Communication
- Deployment window announcements to the team and stakeholders
- Incident alerts, status updates, and post-mortems
- Runbook documentation in the project wiki

### Interactions with Other Roles
- Pair with **Developers** on pipeline reliability and testability of deployment steps
- Coordinate with **Security Lead** on vulnerability scanning and secret management
- Advise **Project Manager** and **Stakeholders** on deployment windows and risk
- Collaborate with **Operations** to ensure smooth production handoff and support tooling
- Work with **QA Lead** on smoke test automation in the deployment pipeline

---

## Data Analyst

### Role Summary
Data Analysts define success metrics, build dashboards, and support data-driven decisions throughout the project lifecycle.

### Responsibilities
- Define and document key performance indicators (KPIs) aligned to project goals
- Instrument and validate event tracking with Developers
- Build and maintain dashboards for feature adoption, usage, and quality signals
- Produce post-release analytics reports and insights
- Advise the team when data suggests scope or priority changes

### Goals
- Enable data-driven prioritization and feature validation
- Reduce time to insight with automated, reliable dashboards
- Ensure metrics are agreed upon before implementation begins

### Typical Communication
- Metrics reviews in sprint demos and milestone check-ins
- Ad-hoc data queries and reports shared in team channels
- KPI documentation in the project one-pager or a linked metrics doc

### Interactions with Other Roles
- Work closely with **Product Manager** to define and validate success metrics
- Support **Developers** with instrumentation specifications and event tracking
- Share adoption and quality signals with **Project Manager** for status reports
- Provide insights to **Stakeholders** during milestone reviews
- Collaborate with **Operations** on support ticket analysis and customer impact metrics

---

## Operations

### Role Summary
Operations team members manage day-to-day business processes and customer-facing support, ensuring a smooth handoff from development to production and sustained service quality post-release.

### Responsibilities
- Develop and maintain support playbooks and runbooks
- Coordinate with the delivery team on rollout communication and readiness
- Manage customer-facing documentation and training materials
- Triage incoming issues and escalate bugs to the development team
- Track operational metrics (e.g., support ticket volume, SLA adherence)

### Goals
- Minimize customer disruption during and after releases
- Ensure support teams are trained and equipped before go-live
- Reduce time to resolve customer-reported issues

### Typical Communication
- Pre-release readiness reviews with PM and SRE/DevOps
- Post-release incident triage and bug escalation
- Regular syncs with QA for known issues and workarounds

### Interactions with Other Roles
- Work with **Project Manager** to align on rollout plans and communication schedules
- Coordinate with **SRE/DevOps** on deployment windows and incident response procedures
- Collaborate with **QA Lead** for release validation and known-issues documentation
- Receive insights from **Data Analyst** for customer impact assessment
- Escalate critical bugs to **Developers** and **Security Lead** as appropriate

---

## QA Lead

### Role Summary
QA Leads coordinate the end-to-end testing strategy and own acceptance sign-off. They ensure quality gates are met before features are released.

### Responsibilities
- Draft and maintain test plans and test cases
- Execute exploratory, regression, and acceptance testing
- Define and sign off on the Definition of Done for each feature or sprint
- Document, track, and prioritize bugs in the issue tracker
- Coordinate UAT with Operations and Stakeholders when needed

### Goals
- Catch defects before they reach production
- Ensure acceptance criteria are verifiable and verified
- Maintain a sustainable, automated test suite

### Typical Communication
- QA status updates in weekly delivery syncs
- Bug reports and test results in the issue tracker
- Go/no-go sign-off communicated to PM before release

### Interactions with Other Roles
- Work with **Developers** to clarify acceptance criteria and unblock test coverage
- Align with **Product Manager** on Definition of Done and acceptance gates
- Consult **Security Lead** to include security test cases in test plans
- Coordinate with **UX Designer** on usability acceptance criteria
- Communicate release readiness status to **Project Manager** and **Operations**

---

## Stakeholder

### Role Summary
Stakeholders provide business requirements, review deliverables, and make key decisions that shape project direction. They are the primary voice of the business or end-user community.

### Responsibilities
- Articulate business goals, constraints, and success criteria
- Review and provide timely feedback on deliverables and demos
- Make or escalate key decisions that affect project scope or priority
- Sign off on major milestones (e.g., initiation, planning, release)
- Champion the project within their area of the business

### Goals
- Ensure the project delivers measurable business value
- Stay informed without being bottlenecked in day-to-day decisions
- Provide clear, timely direction when decisions are needed

### Typical Communication
- Monthly or milestone-based status updates from Project Manager
- Sprint or milestone demos and review sessions
- Escalation calls when project-level decisions are required

### Interactions with Other Roles
- Engaged by **Product Manager** and **Project Manager** at key lifecycle gates
- Provide UX/design feedback to **UX Designer** and **Product Manager**
- Review security or compliance posture with **Security Lead** when required
- Review and approve release readiness with **Project Manager** before major releases

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [Templates & Checklists](./octoacme-templates-and-checklists.md) for a RACI matrix you can populate with these roles for any project.

