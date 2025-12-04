# OctoAcme — Retrospective & Continuous Improvement

**Navigation**: [← Release](octoacme-release-and-deployment.md) | [Overview](octoacme-project-management-overview.md) | [Back to Initiation →](octoacme-project-initiation.md)

## Purpose
Capture learnings and convert them into actionable improvements that feed back into the project lifecycle.

## When
After each sprint, release, or important milestone. Also after incidents.

## Structure
- What went well
- What could be improved
- Action items (owner, due date)
- Follow-up on previous action items

## Running a Retrospective
- Timebox: 45–75 minutes depending on team size
- Use an anonymous idea board if needed to encourage candor
- Prioritize 2–3 top action items to avoid overload

## Tracking Improvements
- Add action items to the project backlog or issues with clear owners and timelines
- Review outstanding actions in the weekly PM sync

## Example Action Item Template
- Title:
- Description:
- Owner:
- Due date:
- Success criteria:

## GitHub Integration for Retrospectives

### Capturing Retrospective Notes
- **Create a retrospective document** in `docs/retros/` folder (e.g., `sprint-42-retro.md`)
- **Use GitHub Issues** to track action items with:
  - Label: `retro-action-item`
  - Clear title describing the improvement
  - Description with context from retrospective
  - Assignee and due date
  - Milestone (for tracking in next sprint/release)
- **Link to the retrospective doc** in action item issues for context

### Retrospective Document Template
```markdown
# Retrospective: [Sprint/Release Name] - [Date]

## Attendees
- List team members who participated

## What Went Well
- [Item 1]
- [Item 2]

## What Could Be Improved
- [Item 1]
- [Item 2]

## Action Items
- [ ] [Action 1] - Owner: [Name] - Due: [Date] - GitHub Issue: #123
- [ ] [Action 2] - Owner: [Name] - Due: [Date] - GitHub Issue: #124

## Follow-up on Previous Action Items
- [x] [Previous action] - Status: Completed
- [ ] [Previous action] - Status: In progress, moved to next sprint

## Key Metrics
- Velocity: [X story points / Y issues completed]
- Cycle time: [Average time from In Progress to Done]
- Bug count: [Number of bugs found/fixed]
- PR review time: [Average review turnaround]

## Notable Achievements
- Celebrate wins and recognize team contributions
```

## Role Responsibilities in Retrospectives

### Scrum Master
- Facilitates the retrospective meeting
- Ensures psychological safety for candid feedback
- Guides the team to prioritize 2-3 actionable improvements
- Creates GitHub Issues for action items
- Follows up on action item progress

### Project Manager
- Participates and provides perspective on cross-team coordination
- Commits to addressing process or communication improvements
- Tracks action items in project tracking
- Reports on metrics and trends

### Team Members (All)
- Reflect on the sprint/release and share honest feedback
- Propose improvements and volunteer to own action items
- Follow through on commitments
- Support teammates' improvement initiatives

## Continuous Improvement Culture
- **Measure impact** of action items using metrics (velocity, quality, morale)
- **Celebrate improvements** and recognize team efforts
- **Make small, iterative changes** rather than large process overhauls
- **Review past retrospectives** to identify patterns and systemic issues
- **Share learnings** with other teams through documentation and presentations
- **Update process docs** based on successful improvements

## Closing the Loop
After the retrospective, the cycle begins again with planning or initiation of the next project:
1. **Action items feed into next sprint backlog** (via GitHub Issues)
2. **Process improvements update documentation** (this doc and others in `docs/`)
3. **Learnings inform risk identification** for future projects
4. **Team capabilities grow** through continuous learning and adaptation

This creates a living, evolving process that improves over time.

→ [Back to Overview](octoacme-project-management-overview.md) | [Start Next Project: Initiation](octoacme-project-initiation.md)

## Tracking Action Items Across Sprints

### Using GitHub Projects for Action Items
- Add `retro-action-item` issues to the project board
- Track status through workflow columns (Backlog → Ready → In Progress → Done)
- Review outstanding action items at the start of each retrospective
- Report on action item completion rate as a process health metric

### Action Item Review Template (for next retrospective)

| Action Item | Owner | Due Date | Status | Outcome/Impact |
|-------------|-------|----------|--------|----------------|
| Improve PR review time | Dev Team | Sprint 43 | ✅ Completed | Average review time reduced from 48h to 18h |
| Add automated security scans | DevOps | Sprint 43 | 🔄 In Progress | Implemented Dependabot, working on CodeQL |
| Clarify acceptance criteria | BA + PM | Sprint 43 | ✅ Completed | All stories now have testable criteria |

## Related Resources
- [Project Management Overview](octoacme-project-management-overview.md) — Full lifecycle context
- [Roles and Personas](octoacme-roles-and-personas.md) — Who does what in retrospectives
- [Execution & Tracking](octoacme-execution-and-tracking.md) — Metrics to review in retrospectives
- [Release & Deployment](octoacme-release-and-deployment.md) — Release-specific learnings to capture
- [Issue Template](.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) — Propose improvements to these process docs
