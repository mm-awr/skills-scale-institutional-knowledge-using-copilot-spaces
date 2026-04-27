# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

> See [Templates & Checklists](./octoacme-templates-and-checklists.md#release-readiness-checklist) for the complete Release Readiness Checklist.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and signed off by **QA Lead** (see [Definition of Done](./octoacme-templates-and-checklists.md#definition-of-done-dod-template))
- Passing CI and security scans — **Security Lead** confirms no critical findings open
- Release notes drafted
- Rollback / mitigation plan documented and reviewed by **SRE/DevOps**
- Smoke tests prepared
- **Operations** runbook / support playbook updated

## Deployment Checklist
- [ ] Deployment window scheduled and confirmed with SRE/DevOps and Operations
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

**Release Readiness Owner:** Project Manager  
**QA sign-off required from:** QA Lead  
**Security sign-off required from:** Security Lead  
**Deployment executed by:** SRE/DevOps

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **SRE/DevOps** triggers incident response and notifies on-call
  - Rollback to last known-good release if necessary — owned by **SRE/DevOps**
  - **Project Manager** notifies **Stakeholders** and **Operations** of the issue and timeline
  - Triage root cause and capture action items — involve **Security Lead** if a security issue is suspected

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
