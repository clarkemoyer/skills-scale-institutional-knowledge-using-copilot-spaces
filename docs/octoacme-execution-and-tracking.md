# OctoAcme — Execution & Tracking

**Navigation**: [← Planning](octoacme-project-planning.md) | [Overview](octoacme-project-management-overview.md) | [Next: Release →](octoacme-release-and-deployment.md)

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
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] **Branching and PR conventions** documented in repo (e.g., CONTRIBUTING.md or README)
- [ ] **CI/CD pipeline** configured for automated tests, linting, and security scans
- [ ] **Daily standups** scheduled and attended by core team (PM, Developers, QA Lead, Scrum Master)
- [ ] **Weekly delivery syncs** scheduled with Product Manager and Stakeholders
- [ ] **Sprint/milestone demos** scheduled (end of sprint or at milestone completion)
- [ ] **Risk register** reviewed and updated weekly by Project Manager
- [ ] **GitHub Project board** updated continuously as work progresses
- [ ] **Blockers escalated** within 24 hours using defined escalation paths
- [ ] **PR review turnaround** monitored (target: <24 hours for reviews)
- [ ] **Metrics tracked** (velocity, burndown, defect rate, cycle time)

## Role Responsibilities in Execution

### Developers
- Move issues through the workflow (Ready → In Progress → In Review → Done)
- Create small, focused PRs with clear descriptions and links to issues
- Write tests and documentation alongside feature code
- Participate in code reviews and provide constructive feedback
- Attend standups and flag blockers early

### QA Lead
- Execute test plans and update test case status
- Log defects as GitHub Issues with clear reproduction steps
- Triage bugs with Product Manager and Developers
- Run regression tests before milestones and releases
- Track quality metrics (test coverage, pass rates, defect trends)

### Scrum Master
- Facilitate daily standups and keep them focused (<15 min)
- Track and remove impediments
- Coach the team on agile practices and process improvements
- Protect the team from disruptions and context switching
- Monitor team health and morale

### Project Manager
- Update stakeholders on progress, risks, and upcoming milestones
- Maintain the Risk Register and escalate critical issues
- Coordinate cross-team dependencies
- Ensure documentation is up to date
- Track metrics and report status

### Product Manager
- Clarify requirements and acceptance criteria as questions arise
- Reprioritize backlog based on new information or feedback
- Review completed work in demos and provide feedback
- Make trade-off decisions on scope and timeline

### UX Designer
- Provide design assets and specifications as needed
- Review implementation for design consistency
- Conduct usability testing and provide feedback
- Update designs based on user feedback and technical constraints

### Business Analyst
- Clarify edge cases and business logic during development
- Validate that implementation meets documented requirements
- Update requirements documentation based on learnings

## GitHub Workflow Details

### Issue Workflow
1. **Backlog** → Issue is prioritized but not ready to start
2. **Ready** → Issue has clear acceptance criteria, is unblocked, and ready to assign
3. **In Progress** → Developer assigns themselves and begins work, creates feature branch
4. **In Review** → PR is created and linked to issue, awaiting code review
5. **QA** → Code is merged to main/dev branch, QA testing begins
6. **Done** → Feature is tested, verified, and ready for release

### Pull Request Best Practices
- **Branch naming**: Use descriptive names (e.g., `feature/add-user-profile`, `fix/login-bug`)
- **PR title**: Clear and concise, reference issue number (e.g., "Add user profile page (#42)")
- **PR description**: Include:
  - Link to issue (e.g., "Closes #42")
  - Summary of changes
  - Acceptance criteria checklist
  - Testing approach
  - Screenshots (for UI changes)
- **Small PRs**: Aim for ≤400 lines changed; break large features into smaller PRs
- **CI checks**: Ensure all automated tests, linting, and security scans pass before requesting review
- **Review requirements**: At least 1 approval (or team-defined policy)
- **Review turnaround**: Reviewers should respond within 24 hours
- **Address feedback**: Respond to all comments, either implementing changes or discussing alternatives

### Labeling Strategy
Use labels to categorize and filter issues and PRs:
- **Type**: `feature`, `bug`, `technical-debt`, `documentation`, `security`
- **Size**: `size:small`, `size:medium`, `size:large` (for estimation)
- **Priority**: `priority:critical`, `priority:high`, `priority:medium`, `priority:low`
- **Status**: `blocked`, `needs-review`, `ready-for-qa`, `in-progress`
- **Component**: `frontend`, `backend`, `api`, `infrastructure` (project-specific)

## Communication Rhythms

### Daily Standup (15 minutes)
**Attendees**: Developers, QA Lead, Scrum Master, Project Manager (optional: Product Manager)
**Format**:
- What did I complete yesterday?
- What am I working on today?
- Any blockers or dependencies?

**Best Practices**:
- Stay focused on progress and blockers, not solutions
- Take detailed discussions offline
- Update GitHub Project board before standup
- Scrum Master tracks blockers and follows up

### Weekly Delivery Sync (30-60 minutes)
**Attendees**: Project Manager, Product Manager, Scrum Master, Tech Lead, QA Lead
**Agenda**:
- Review progress toward milestone (burndown, velocity)
- Discuss completed work and upcoming priorities
- Review and update Risk Register
- Identify scope adjustments or trade-offs
- Plan for upcoming sprint/iteration

### Sprint/Milestone Demo (30-60 minutes)
**Attendees**: Full team + Stakeholders
**Format**:
- Demo completed features (show, don't tell)
- Gather feedback from stakeholders
- Celebrate wins and acknowledge team contributions
- Preview upcoming work

## Handoff to Release
As the milestone or sprint nears completion, prepare for release:
- [ ] All "Done" items meet Definition of Done
- [ ] Regression testing completed by QA Lead
- [ ] Release notes drafted (see Release & Deployment guide)
- [ ] Rollback plan documented
- [ ] Deployment checklist prepared
- [ ] Stakeholders notified of upcoming release

→ [Next: Release & Deployment Guide](octoacme-release-and-deployment.md)

## Related Resources
- [Project Management Overview](octoacme-project-management-overview.md) — Full lifecycle context
- [Roles and Personas](octoacme-roles-and-personas.md) — Who does what during execution
- [Risk Management & Communication](octoacme-risks-and-communication.md) — Blocker escalation and risk management
- [Release & Deployment](octoacme-release-and-deployment.md) — What happens next
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) — Capturing learnings
