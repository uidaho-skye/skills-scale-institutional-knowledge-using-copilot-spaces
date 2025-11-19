# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- **Identify**: during planning and ongoing execution
  - **PM**, **Business Analyst**, **QA Lead**, and **Developers** identify risks
- **Assess**: estimate impact and likelihood
  - **PM** coordinates assessment with subject matter experts
- **Mitigate**: reduced via actions, contingency plans
  - Risk owner (assigned by **PM**) executes mitigation plan
- **Monitor**: review at weekly syncs and update status
  - **PM** reviews with team, **Change Manager** assesses if changes needed

## Stakeholder Communication
- **PM** identifies stakeholder groups and communication needs (e.g., engineering, sales, support)
- **PM** and **Release Coordinator** provide regular updates (weekly or milestone-based)
- **Business Analyst** communicates requirements changes to stakeholders
- Use a single source of truth (project README or release doc) for status

## Communication Templates

### Weekly Status Template:
Prepared by **PM** with input from team:

- **Progress this week**:
- **Next steps**:
- **Risks & blockers**:
- **Quality status** (from **QA Lead**):
- **Ask / decisions needed**:

### Incident Communication
Led by **Release Coordinator** (for deployment incidents) or **PM** (for project incidents):

- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level → **PM** → **Product Lead** → Sponsor
- For scope/timeline changes → **Change Manager** → CAB (if needed)
- For security incidents, follow the security incident runbook and notify Security on-call
- For release issues → **Release Coordinator** → **PM** → On-call team
