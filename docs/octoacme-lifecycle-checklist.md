# OctoAcme — Project Lifecycle Checklist

**Navigation**: [Overview](octoacme-project-management-overview.md) | [All Process Docs](README.md)

## Purpose
This checklist provides a comprehensive view of the OctoAcme project lifecycle, showing key activities, artifacts, decision gates, and role responsibilities across all phases. Use it as a roadmap to ensure nothing is missed as projects progress from initiation through retrospective.

---

## Phase 1: Initiation

### Goals
- Validate business need and measurable outcomes
- Align stakeholders on problem and priorities
- Secure approval to proceed to planning

### Key Activities
- [ ] Conduct initial discovery and problem analysis
- [ ] Draft Project One-pager with problem, goals, metrics, timeline
- [ ] Identify stakeholders and decision makers
- [ ] Assess initial risks and dependencies
- [ ] Estimate resource requirements
- [ ] Create GitHub repository (if new) and project board
- [ ] Present to sponsor/stakeholders for approval

### Key Artifacts
- **Project One-pager** ([template](octoacme-project-onepager-template.md))
- Stakeholder list and communication plan
- Initial risk list (top 3-5 risks)
- High-level timeline with major milestones

### Role Responsibilities
- **Product Manager**: Defines problem, success metrics, business value
- **Project Manager**: Facilitates initiation, coordinates stakeholders, drafts timeline
- **Business Analyst**: Helps clarify requirements and document initial scope
- **Stakeholders**: Provide input, validate business need, approve/reject
- **Sponsor**: Makes go/no-go decision

### Decision Gate: Initiation → Planning
**Criteria**:
- [ ] Problem statement is clear and compelling
- [ ] Success metrics are defined and measurable
- [ ] Stakeholders agree on priority
- [ ] Team availability is confirmed
- [ ] Sponsor has approved moving to planning

**Decision Makers**: Sponsor (approve), Product Manager (recommend), Stakeholders (input)

**Next Step**: Schedule planning kickoff → [Planning Phase](#phase-2-planning)

---

## Phase 2: Planning

### Goals
- Create actionable backlog with acceptance criteria
- Identify all dependencies and risks
- Establish Definition of Done and release timeline
- Prepare team to start execution

### Key Activities
- [ ] Conduct planning kickoff with full team
- [ ] Break work into user stories/issues with acceptance criteria
- [ ] Estimate scope (story points, t-shirt sizes)
- [ ] Define Definition of Done (DoD)
- [ ] Create formal Risk Register with mitigation plans
- [ ] Identify and document dependencies
- [ ] Create release plan with sprints/milestones
- [ ] Set up GitHub Issues, labels, and project board columns
- [ ] Establish communication cadence (standups, syncs, demos)
- [ ] Define PR and branching conventions
- [ ] Set up CI/CD pipeline (tests, linting, security scans)

### Key Artifacts
- **Prioritized backlog** (GitHub Issues in project board)
- **Definition of Done** (documented in repo or project docs)
- **Risk Register** ([see template](octoacme-risks-and-communication.md))
- **Release plan** with milestones (GitHub Milestones)
- **Test strategy** (coordinated by QA Lead)
- **Communication plan** (meeting schedule, channels)

### Role Responsibilities
- **Product Manager**: Prioritizes backlog, clarifies requirements, defines acceptance criteria
- **Project Manager**: Facilitates planning, manages timeline, tracks dependencies
- **Scrum Master**: Coaches on estimation, ensures DoD is clear, facilitates ceremonies
- **Business Analyst**: Documents detailed requirements, acceptance criteria, edge cases
- **QA Lead**: Defines test strategy, identifies QA dependencies and risks
- **UX Designer**: Provides design specs, clarifies UI/UX acceptance criteria
- **Developers**: Estimate effort, identify technical risks and dependencies
- **Stakeholders**: Review plan, provide input on priorities and constraints

### Decision Gate: Planning → Execution
**Criteria**:
- [ ] Backlog has at least 1-2 sprints of "Ready" work
- [ ] All "Ready" issues have clear acceptance criteria
- [ ] Definition of Done is documented and agreed upon
- [ ] Major dependencies are identified with mitigation plans
- [ ] Risk Register is created and reviewed
- [ ] CI/CD pipeline is configured
- [ ] Team members understand roles and communication cadence

**Decision Makers**: Project Manager (confirm readiness), Product Manager (approve priorities), Team (commit to plan)

**Next Step**: Begin first sprint → [Execution Phase](#phase-3-execution--tracking)

---

## Phase 3: Execution & Tracking

### Goals
- Build, test, and deliver features incrementally
- Track progress and manage blockers
- Maintain quality through testing and code review
- Keep stakeholders informed

### Key Activities
- [ ] Conduct daily standups (progress, blockers, priorities)
- [ ] Move issues through workflow (Backlog → Ready → In Progress → Review → QA → Done)
- [ ] Create and review pull requests (small, linked to issues, with tests)
- [ ] Run CI/CD checks (tests, linting, security scans)
- [ ] Execute test plans (unit, integration, e2e)
- [ ] Update GitHub Project board continuously
- [ ] Review and update Risk Register weekly
- [ ] Hold weekly delivery syncs (status, risks, decisions)
- [ ] Conduct sprint/milestone demos for stakeholders
- [ ] Escalate blockers within 24 hours if unresolved
- [ ] Track metrics (velocity, burndown, cycle time, quality)

### Key Artifacts
- **GitHub Project board** (continuously updated)
- **Pull requests** with acceptance criteria and tests
- **Test results** (CI/CD reports, QA test cases)
- **Risk Register updates** (weekly or as risks emerge)
- **Weekly status updates** (to stakeholders)
- **Demo recordings or notes** (from sprint reviews)

### Role Responsibilities
- **Developers**: Implement features, write tests, review code, update issues
- **QA Lead**: Execute tests, log bugs, triage defects, track quality metrics
- **Scrum Master**: Facilitate standups, remove blockers, coach team on process
- **Project Manager**: Track progress, manage risks, communicate status, coordinate dependencies
- **Product Manager**: Clarify requirements, reprioritize backlog, review demos, make trade-offs
- **UX Designer**: Provide design assets, review implementation, conduct usability tests
- **Business Analyst**: Clarify edge cases, validate requirements, update documentation
- **Stakeholders**: Attend demos, provide feedback, approve scope changes

### Continuous Checkpoints (throughout execution)
- [ ] All PRs reviewed within 24 hours
- [ ] Blockers escalated within 24 hours
- [ ] Risk Register updated weekly
- [ ] GitHub Project board reflects reality
- [ ] Quality metrics tracked and improving
- [ ] Team morale healthy (check-ins with Scrum Master)

**Next Step**: When milestone is complete → [Release Phase](#phase-4-release--deployment)

---

## Phase 4: Release & Deployment

### Goals
- Deploy features to production safely
- Verify release meets acceptance criteria
- Communicate changes to users and stakeholders
- Prepare for rollback if needed

### Key Activities
- [ ] Verify all acceptance criteria are met
- [ ] Complete regression testing in staging
- [ ] Draft release notes with all changes
- [ ] Document rollback plan
- [ ] Prepare post-deployment smoke tests
- [ ] Schedule deployment window (if needed)
- [ ] Create GitHub Release with tag and notes
- [ ] Deploy to staging and verify
- [ ] Get sign-off from QA Lead and Product Manager
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deployment verification and smoke tests
- [ ] Monitor metrics, logs, and alerts
- [ ] Announce release to stakeholders and users
- [ ] Update status page or dashboard

### Key Artifacts
- **Release notes** ([see template](octoacme-release-and-deployment.md))
- **GitHub Release** (with tag, notes, linked PRs/issues)
- **Rollback plan** (documented procedures)
- **Post-deployment checklist** (smoke tests, verification)
- **Release announcement** (to stakeholders and users)

### Role Responsibilities
- **Project Manager**: Coordinates release timeline, communicates status, coordinates rollback if needed
- **Product Manager**: Approves release, reviews notes, plans user communication
- **QA Lead**: Executes final testing, runs smoke tests, signs off on release readiness
- **Developers**: Ensure code is deployable, monitor deployment, fix issues if needed
- **Scrum Master**: Facilitates release retrospective, tracks process improvements
- **Stakeholders**: Approve release (if required), prepare their teams for changes

### Decision Gate: Release → Retrospective
**Criteria**:
- [ ] All features deployed successfully
- [ ] Smoke tests passed
- [ ] No critical production issues
- [ ] Stakeholders notified
- [ ] Metrics show expected behavior

**Decision Makers**: QA Lead (quality sign-off), Product Manager (approve), Project Manager (coordinate)

**Next Step**: Schedule retrospective within 1-3 days → [Retrospective Phase](#phase-5-retrospective--continuous-improvement)

---

## Phase 5: Retrospective & Continuous Improvement

### Goals
- Capture what went well and what could improve
- Create actionable improvements with owners
- Close project loop and prepare for next iteration

### Key Activities
- [ ] Schedule retrospective within 1-3 days of release
- [ ] Prepare metrics and data (velocity, quality, cycle time)
- [ ] Facilitate retrospective meeting (Scrum Master)
- [ ] Identify what went well
- [ ] Identify what could improve
- [ ] Prioritize 2-3 actionable improvement items
- [ ] Create GitHub Issues for action items with owners and due dates
- [ ] Review previous retro action items (what was completed?)
- [ ] Document retrospective notes in `docs/retros/` folder
- [ ] Update process documentation based on learnings
- [ ] Celebrate wins and recognize team contributions
- [ ] Close project milestone in GitHub

### Key Artifacts
- **Retrospective notes** ([see template](octoacme-retrospective-and-continuous-improvement.md))
- **Action items** (GitHub Issues with `retro-action-item` label)
- **Updated process documentation** (if improvements change processes)
- **Metrics summary** (velocity, quality, cycle time for this project)

### Role Responsibilities
- **Scrum Master**: Facilitates retrospective, creates action item issues, follows up on progress
- **Project Manager**: Provides perspective on coordination and stakeholder management
- **Team Members (All)**: Reflect honestly, propose improvements, volunteer for action items
- **Product Manager**: Shares perspective on business value delivered vs. planned
- **QA Lead**: Provides quality metrics and testing insights

### Closing the Loop
- [ ] Action items added to next sprint/project backlog
- [ ] Process documentation updated (if applicable)
- [ ] Learnings shared with other teams (if applicable)
- [ ] Team achievements celebrated
- [ ] Project marked as "Closed" in GitHub

**Next Step**: Begin next project with Initiation phase → [Phase 1: Initiation](#phase-1-initiation)

---

## Cross-Phase Best Practices

### GitHub as System of Record
- **Issues**: All work items, bugs, decisions, risks tracked as issues
- **Projects**: Visual workflow board (Backlog → Ready → In Progress → Review → QA → Done)
- **Pull Requests**: Small, linked to issues, include acceptance criteria and tests
- **Releases**: Tagged releases with comprehensive notes and linked PRs/issues
- **Documentation**: All process docs and project artifacts in `docs/` folder
- **Milestones**: Group issues by release or sprint for planning and tracking

### Copilot Spaces Integration
- Keep relevant process docs in `.copilot/` directory for AI context
- Sync changes between `docs/` and `.copilot/` when updating processes
- Use Copilot Spaces to answer questions about processes and standards
- Reference this lifecycle checklist in Copilot Space for guidance

### Risk Management Throughout
- **Initiation**: Identify top 3-5 initial risks
- **Planning**: Create formal Risk Register with mitigation plans
- **Execution**: Update Risk Register weekly, escalate new risks immediately
- **Release**: Assess deployment risks, prepare rollback plans
- **Retrospective**: Review how risks materialized, update risk practices

### Communication Throughout
- **Initiation**: Align stakeholders on problem and goals
- **Planning**: Set communication cadence and expectations
- **Execution**: Daily standups, weekly syncs, sprint demos
- **Release**: Release announcements and user communication
- **Retrospective**: Share learnings with broader team

### Quality Throughout
- **Initiation**: Define success metrics
- **Planning**: Define Definition of Done, test strategy
- **Execution**: Continuous testing, code review, CI/CD checks
- **Release**: Regression testing, smoke tests, monitoring
- **Retrospective**: Review quality metrics, improve processes

---

## Using This Checklist

### For New Projects
1. Start at Phase 1 (Initiation) and work through each phase sequentially
2. Check off items as they're completed
3. Use decision gates to ensure readiness before moving to next phase
4. Customize checklist based on project size and complexity

### For In-Flight Projects
1. Identify your current phase
2. Review checklist items for that phase to ensure nothing is missed
3. Look ahead to next phase to prepare
4. Look back to previous phases to verify foundational work is complete

### For Process Improvement
1. Use this checklist in retrospectives to identify gaps
2. Propose changes to this checklist via the [issue template](.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml)
3. Continuously refine based on team learnings

---

## Related Resources

### Phase-Specific Guides
- [Project Initiation](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Release & Deployment](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)

### Supporting Documentation
- [Project Management Overview](octoacme-project-management-overview.md)
- [Roles and Personas](octoacme-roles-and-personas.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
- [Project One-pager Template](octoacme-project-onepager-template.md)

### GitHub Resources
- [Issue Template for Process Doc Updates](.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml)
- [Complete Process Documentation](README.md)
