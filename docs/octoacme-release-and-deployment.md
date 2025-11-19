# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability. The **Release Coordinator** orchestrates this process in collaboration with the team.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- **QA Lead sign-off**: Quality gates met, testing complete
- **Change Manager approval**: All changes reviewed and approved (if applicable)
- **Release Coordinator verification**: Release readiness checklist complete
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
**Release Coordinator** leads this process with team support:

- [ ] Deployment window scheduled and communicated (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] **QA Lead**: Validate staging environment
- [ ] **PM**: Confirm go/no-go decision
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] **Release Coordinator**: Announce release to stakeholders and support
- [ ] **Change Manager**: Update change logs (if applicable)

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **Release Coordinator**: Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - **PM and QA Lead**: Triage root cause and capture action items
  - **Change Manager**: Update change records with incident details

## Release Notes Template
**Release Coordinator** prepares with input from team:

- **Release name / number**:
- **Date**:
- **Summary**:
- **Notable changes**:
- **Migration steps (if any)**:
- **Known issues**:

## Key Hand-offs
- **Developers → QA Lead**: Code complete, ready for final testing
- **QA Lead → Release Coordinator**: Quality sign-off, release approved
- **Change Manager → Release Coordinator**: Change approvals confirmed
- **Release Coordinator → Stakeholders**: Release communication and notes
- **PM → All**: Go/no-go decision based on readiness criteria
