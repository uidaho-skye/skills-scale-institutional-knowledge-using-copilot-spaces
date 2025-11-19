# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- **QA Lead** develops and maintains testing strategy
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed
- **Hand-off**: Developers notify QA Lead when PRs are ready for testing
- **Hand-off**: QA Lead signs off on release readiness to Release Coordinator

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- **Level 1**: Team-level triage in daily standup
- **Level 2**: PM escalates to Product Lead and dependent teams
- **Level 3**: Sponsor-level escalation for business-impacting issues
- **Change-related**: Change Manager evaluates if scope/timeline adjustments needed

## Role-Specific Responsibilities During Execution

### Business Analyst
- Clarify requirements and acceptance criteria as questions arise
- Validate that implementation aligns with business objectives
- Update use cases and documentation based on learnings

### QA Lead
- Review test coverage weekly
- Triage defects and work with developers on prioritization
- Report testing status and quality metrics in delivery sync

### Change Manager (when applicable)
- Review incoming change requests and assess impact
- Communicate approved changes to team
- Ensure change documentation is updated

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] QA Lead notified when features ready for testing
- [ ] Business Analyst available for requirements clarification
