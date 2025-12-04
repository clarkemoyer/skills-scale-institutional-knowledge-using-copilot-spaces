# OctoAcme — Project Planning

**Navigation**: [← Initiation](octoacme-project-initiation.md) | [Overview](octoacme-project-management-overview.md) | [Next: Execution →](octoacme-execution-and-tracking.md)

## Purpose
Turn an approved initiative into an actionable plan and backlog for delivery.

## Objectives
- Break work into shippable increments
- Identify dependencies and risks
- Align timelines, releases, and responsibilities

## Activities
1. Kickoff meeting with stakeholders and delivery team
2. Create prioritized backlog with acceptance criteria
3. Estimate scope (T-shirt sizing or story points)
4. Define Definition of Done (DoD)
5. Identify dependencies and integration points
6. Create release plan and milestone map

## Backlog Item Template
- Title:
- Description:
- Acceptance criteria:
- Priority:
- Estimate:
- Owner:
- Related docs/links:

## Sprint / Iteration Planning
- Timebox planning to agreed sprint length
- Pull items that meet DoD and have clear acceptance criteria
- Ensure team capacity is respected

## Risk & Dependency Management
- Capture in Risk Register:
  - ID, Description, Impact, Probability, Owner, Mitigation
- Mark cross-team dependencies in the project board and escalate during weekly syncs

## Planning Checklist
- [ ] Project kickoff held (attendees: PM, PdM, Developers, QA Lead, UX Designer, Stakeholders)
- [ ] Backlog prioritized and estimated (using GitHub Issues and Project board)
- [ ] Release timeline and milestones agreed (documented in Project board milestones)
- [ ] Definition of Done documented (in repo README or project docs)
- [ ] Initial test plan / QA approach drafted (coordinated by QA Lead)
- [ ] Dependencies identified and tracked (in Risk Register and GitHub Issues)
- [ ] Acceptance criteria defined for each backlog item (in Issue descriptions)
- [ ] Team capacity assessed and sprint/iteration length agreed
- [ ] Communication cadence established (standups, syncs, demos)

## GitHub Integration for Planning
- **GitHub Issues**: Create issues for all backlog items with:
  - Clear title and description
  - Acceptance criteria in the issue body
  - Labels (feature, bug, technical-debt, etc.)
  - Size/estimate (use labels like `size:small`, `size:medium`, `size:large`)
  - Assignee (when ready to start)
  - Milestone (if using milestone-based planning)
- **GitHub Projects**: Organize issues in project board columns:
  - Backlog: Prioritized but not yet ready
  - Ready: Clear acceptance criteria, unblocked, ready to start
  - In Progress: Active development
  - In Review: PR open and under review
  - QA: Testing and validation
  - Done: Merged and verified
- **GitHub Milestones**: Use milestones to group issues by release or sprint
- **Dependencies**: Use issue references (e.g., "Blocked by #123") and task lists within issues

## Role Responsibilities in Planning

### Product Manager
- Prioritizes the backlog based on customer value and business impact
- Defines success metrics for the release
- Clarifies requirements and acceptance criteria with the Business Analyst

### Project Manager
- Facilitates the planning kickoff and ongoing planning sessions
- Tracks dependencies and risks in the Risk Register
- Ensures the release timeline is realistic and communicated

### Scrum Master
- Guides the team on estimation practices (story points, t-shirt sizes)
- Ensures the Definition of Done is clear and achievable
- Coaches the team on breaking down work into small, deliverable increments

### Business Analyst
- Documents detailed acceptance criteria and edge cases
- Maps dependencies between work items
- Ensures requirements are testable and complete

### QA Lead
- Defines the test strategy and approach
- Identifies testing dependencies and risks
- Estimates QA effort and coordinates test environment needs

### UX Designer
- Provides design specifications and prototypes
- Collaborates on acceptance criteria for UI/UX features
- Identifies design dependencies and timeline

### Developers
- Estimate effort for technical work
- Identify technical risks and dependencies
- Propose technical approaches and architecture decisions

## Decision Gate
Move to execution when:
- Backlog has at least 1-2 sprints of "Ready" work with clear acceptance criteria
- Team has agreed on Definition of Done
- Major dependencies are identified and mitigation plans exist
- All team members understand their roles and the communication cadence

**Decision Makers**: Project Manager (confirm readiness), Product Manager (approve priorities), Team (commit to plan)

## Handoff to Execution
Before starting execution, ensure:
- GitHub Project board is up to date with prioritized issues
- First sprint/iteration is planned with team capacity in mind
- Standup and sync meetings are scheduled
- All team members have access to repo, project board, and documentation
- Risks are documented and escalation paths are clear

→ [Next: Execution & Tracking Guide](octoacme-execution-and-tracking.md)

## Related Resources
- [Project Management Overview](octoacme-project-management-overview.md) — Full lifecycle context
- [Roles and Personas](octoacme-roles-and-personas.md) — Who does what during planning
- [Risk Management & Communication](octoacme-risks-and-communication.md) — Risk and dependency management
- [Execution & Tracking](octoacme-execution-and-tracking.md) — What happens next
