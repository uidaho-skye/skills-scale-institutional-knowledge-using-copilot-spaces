# OctoAcme — Change Management Process

## Purpose
Define how OctoAcme evaluates, approves, and implements changes to projects, systems, and processes to minimize disruption while enabling necessary adaptations.

## Scope
This process applies to:
- Scope changes to active projects
- Changes to production systems or infrastructure
- Process or policy modifications
- Emergency/urgent changes requiring expedited approval

## Roles and Responsibilities

### Change Manager
- Evaluate and prioritize change requests
- Assess impact on projects, systems, and stakeholders
- Coordinate Change Advisory Board (CAB) when needed
- Communicate decisions and track implementation
- Maintain change logs and compliance

### Project Manager
- Submit change requests for project scope/timeline impacts
- Implement approved changes to project plans
- Communicate change impacts to team and stakeholders

### Business Analyst
- Assess business impact of proposed changes
- Update requirements documentation to reflect approved changes
- Validate that changes align with business objectives

### Technical Leads / Developers
- Provide technical impact assessment
- Implement approved technical changes
- Document technical changes and dependencies

## Change Request Process

### 1. Submit Change Request
Use the template below to document the change:

**Change Request Template:**
- **Change ID**: (auto-assigned or use format: CR-YYYY-MM-DD-###)
- **Requestor**: Name and role
- **Date Submitted**: 
- **Type**: [Scope Change | Technical Change | Process Change | Emergency]
- **Priority**: [Low | Medium | High | Critical]
- **Summary**: Brief description of the change
- **Justification**: Why is this change needed?
- **Impact Assessment**:
  - Scope impact: 
  - Schedule impact:
  - Resource impact:
  - Risk impact:
  - Affected systems/teams:
- **Implementation Plan**: How will the change be implemented?
- **Rollback Plan**: How to revert if needed?
- **Stakeholders to notify**:

### 2. Impact Assessment
**Change Manager** reviews with relevant stakeholders:
- Technical feasibility (with developers/leads)
- Business impact (with Business Analyst, Product Manager)
- Schedule/resource impact (with Project Manager)
- Risk evaluation

### 3. Approval Decision
**Change approval levels:**

| Change Type | Approver | Response Time |
|-------------|----------|---------------|
| Low impact (minor updates) | Project Manager | 1-2 business days |
| Medium impact (scope/timeline adjustments) | Change Manager + PM/PdM | 2-5 business days |
| High impact (significant scope/architecture) | CAB (Change Manager, PM, PdM, Technical Lead) | 1 week |
| Emergency/Critical | Expedited CAB review | 24 hours |

### 4. Communication
Once approved or rejected:
- Change Manager notifies requestor and affected stakeholders
- Project Manager updates project documentation if applicable
- Business Analyst updates requirements if applicable
- Release Coordinator updates release plans if applicable

### 5. Implementation & Tracking
- Assigned owner implements the change
- Progress tracked in change log
- Post-implementation review conducted for high-impact changes

## Change Advisory Board (CAB)

### When to convene CAB
- High-impact changes affecting multiple teams or systems
- Changes with significant risk or uncertainty
- Contested changes requiring leadership decision
- Emergency changes (post-implementation review)

### CAB Members
- Change Manager (chair)
- Project Manager
- Product Manager
- Technical Lead or Architect
- Business Analyst (as needed)
- Other stakeholders as relevant

### CAB Meeting Agenda
1. Review pending change requests
2. Impact assessment presentations
3. Discussion and questions
4. Approval decisions
5. Communication and next steps

## Change Log Template

Maintain a change log for each project:

| Change ID | Date | Type | Summary | Status | Approver | Implementation Date | Notes |
|-----------|------|------|---------|--------|----------|---------------------|-------|
| CR-2024-01-15-001 | 2024-01-15 | Scope | Add user export feature | Approved | Change Manager | 2024-01-22 | Successfully implemented |

## Emergency Change Process

For critical production issues requiring immediate action:

1. **Initiate**: On-call team identifies need for emergency change
2. **Assess**: Quick impact assessment with available stakeholders
3. **Approve**: Expedited approval from Change Manager or designee
4. **Implement**: Execute change with careful monitoring
5. **Review**: Post-implementation CAB review within 48 hours
6. **Document**: Update change log with lessons learned

## Best Practices

- **Submit early**: Request changes as soon as need is identified
- **Be specific**: Provide detailed impact assessment and justification
- **Consider alternatives**: Include options and trade-offs
- **Document thoroughly**: Maintain clear records for audit and learning
- **Communicate proactively**: Keep stakeholders informed throughout the process
- **Learn continuously**: Conduct post-implementation reviews on significant changes

## Change Management Checklist

For Project Managers submitting a change:

- [ ] Change request form completed with all required fields
- [ ] Impact assessment conducted with relevant stakeholders
- [ ] Alternative solutions considered and documented
- [ ] Stakeholders identified and notified
- [ ] Submitted to Change Manager for review
- [ ] Approval received before implementation
- [ ] Project documentation updated to reflect approved change
- [ ] Change logged in project change register
- [ ] Post-implementation review scheduled (for high-impact changes)

## Integration with Other Processes

- **Project Initiation**: Establish change management approach during project kickoff
- **Execution & Tracking**: Monitor for scope creep and trigger change process as needed
- **Release & Deployment**: Coordinate approved changes with release schedule
- **Retrospectives**: Review change management effectiveness and improve
