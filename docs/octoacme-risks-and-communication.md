# OctoAcme — Risk Management & Communication

**Navigation**: [Overview](octoacme-project-management-overview.md) | [Related: All lifecycle phases](octoacme-project-management-overview.md#lifecycle-high-level)

## Purpose
Explain how to identify, manage, and communicate risks and dependencies throughout the entire project lifecycle—from initiation through retrospective.

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

Risk management is continuous throughout the project:

### During Initiation
- Identify initial risks in the Project One-pager
- Focus on high-level business, resource, and schedule risks
- Use risks to inform go/no-go decision
- Document top 3-5 risks in the initiation checklist

### During Planning
- Create formal Risk Register with detailed assessment
- Identify technical risks, dependencies, and integration challenges
- Assign risk owners and mitigation plans
- Review risks in planning kickoff with full team

### During Execution
- Update Risk Register weekly during delivery syncs
- Monitor for new risks emerging from execution
- Escalate critical risks immediately (don't wait for weekly sync)
- Track risk mitigation actions in GitHub Issues

### During Release
- Assess deployment risks and prepare rollback plans
- Document incident response procedures
- Identify monitoring and verification steps
- Review past release incidents to prevent recurrence

### During Retrospective
- Review how risks materialized (or didn't)
- Capture lessons learned about risk identification and mitigation
- Update process documentation based on risk learnings
- Add action items to improve future risk management

## Risk Identification by Phase

| Phase | Common Risk Categories | Key Questions |
|-------|------------------------|---------------|
| **Initiation** | Business need unclear, stakeholder misalignment, resource unavailability | Is the problem well-defined? Do stakeholders agree on priority? Are resources committed? |
| **Planning** | Scope creep, technical unknowns, dependency chains, unrealistic estimates | Is scope clear and bounded? Are dependencies identified? Is the timeline realistic? |
| **Execution** | Blockers, quality issues, team velocity, external changes | Are blockers being resolved quickly? Is quality acceptable? Is velocity sustainable? |
| **Release** | Deployment failures, production incidents, rollback needs, user impact | Is the rollback plan tested? Are monitoring alerts configured? Is support ready? |
| **Retrospective** | Lessons not captured, action items not tracked, same mistakes repeated | Are improvements being implemented? Is the team learning from incidents? |

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths

### Standard Escalation (Delivery Blockers, Schedule Risks)
1. **Level 1 - Team**: Discussed in daily standup, Scrum Master tracks and attempts resolution
2. **Level 2 - Project Manager**: If unresolved after 24 hours, PM escalates to Product Lead and dependent teams
3. **Level 3 - Sponsor**: For business-impacting issues, PM escalates to sponsor/executive level

**Timeline**: Escalate within 24 hours if blocker cannot be resolved at team level.

### Critical Escalation (Production Incidents, Security Issues)
1. **Immediate**: Notify on-call engineer and Project Manager
2. **Security incidents**: Follow security incident runbook, notify Security on-call immediately
3. **Production incidents**: Trigger incident response, notify stakeholders per communication plan
4. **Blameless postmortem**: Schedule within 48 hours of incident resolution

### Dependency Escalation
- **Internal dependencies**: PM coordinates with other Project Managers
- **External dependencies**: PM escalates to Product Lead or sponsor to engage external teams
- **Technical dependencies**: Tech Lead or Scrum Master works with other engineering teams

## GitHub Integration for Risk Management

### Using GitHub Issues for Risk Tracking
- Create issues with label `risk` for significant project risks
- Use issue description template:
  - **Risk ID**: Unique identifier (e.g., RISK-001)
  - **Description**: What is the risk?
  - **Impact**: High/Medium/Low - what happens if this risk materializes?
  - **Likelihood**: High/Medium/Low - how likely is it to occur?
  - **Owner**: Who is responsible for monitoring and mitigating?
  - **Mitigation Plan**: What actions reduce this risk?
  - **Status**: Open, Mitigating, Closed, Materialized
- Link risk issues to related work items
- Reference risk issues in weekly status updates

### Risk Register Template (GitHub Issue or Project Doc)

| Risk ID | Description | Impact | Likelihood | Owner | Mitigation Plan | Status | Last Updated |
|---------|-------------|--------|------------|-------|-----------------|--------|--------------|
| RISK-001 | External API integration untested | High | Medium | Dev Lead | Set up test environment, run integration tests by Sprint 2 | Mitigating | 2024-12-01 |
| RISK-002 | Design review delayed, blocks implementation | Medium | Low | UX Designer | Buffer 1 week in schedule, parallelize other work | Open | 2024-12-01 |
| RISK-003 | Third-party dependency upgrade breaks compatibility | High | Medium | Developer | Test in staging, have rollback plan, schedule during low-traffic window | Open | 2024-12-01 |

### Communication Through GitHub
- **Project board comments**: Use for quick updates and questions
- **PR comments**: Discuss implementation details and trade-offs
- **Issue comments**: Document decisions, blockers, and status updates
- **Commit messages**: Reference issues for traceability
- **Release notes**: Summarize changes for stakeholders

## Stakeholder Communication Matrix

| Stakeholder Group | Communication Method | Frequency | Content | Owner |
|-------------------|----------------------|-----------|---------|-------|
| **Delivery Team** | Daily standup | Daily | Progress, blockers, priorities | Scrum Master |
| **Product Manager** | Weekly sync | Weekly | Backlog priorities, scope changes | Project Manager |
| **Sponsors/Executives** | Status email/dashboard | Monthly | High-level progress, major risks | Project Manager |
| **Dependent Teams** | Cross-team sync | As needed | Dependencies, integration points | Project Manager |
| **Stakeholders** | Milestone demos | Per sprint/milestone | Completed features, upcoming work | Product Manager |
| **Support Team** | Release notes | Per release | New features, known issues, workarounds | Project Manager |
| **All Interested Parties** | GitHub Project board | Continuous | Real-time status, work items | All team members |

## Communication Best Practices
- **Single source of truth**: Use GitHub for all project artifacts and status
- **Proactive updates**: Don't wait for stakeholders to ask; provide regular updates
- **Context matters**: Tailor communication style and detail level to audience
- **Document decisions**: Capture key decisions in issues or docs for future reference
- **Escalate early**: If a risk becomes a blocker, escalate within 24 hours
- **Celebrate wins**: Share successes with the team and stakeholders to maintain momentum

## Related Resources
- [Project Initiation](octoacme-project-initiation.md) — Risk identification at project start
- [Project Planning](octoacme-project-planning.md) — Creating the Risk Register
- [Execution & Tracking](octoacme-execution-and-tracking.md) — Monitoring risks during delivery
- [Release & Deployment](octoacme-release-and-deployment.md) — Deployment risk management
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) — Learning from risks that materialized
