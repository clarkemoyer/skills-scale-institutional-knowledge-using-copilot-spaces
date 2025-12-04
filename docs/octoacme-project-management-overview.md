# OctoAcme Project Management Overview

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Manager (PdM).
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles
- **Project Manager (PM)**: coordinates delivery, schedules, risk, communications.
- **Product Manager (PdM)**: defines outcomes, prioritizes backlog, and measures success.
- **Developers**: implement features, collaborate on design and testability.
- **QA Lead**: coordinates testing, quality metrics, and release readiness.
- **Scrum Master**: facilitates agile ceremonies, removes blockers, coaches the team.
- **UX Designer**: designs user experiences, validates usability, maintains design standards.
- **Business Analyst**: translates business needs into requirements, documents criteria.
- **Stakeholders**: provide inputs, approvals, and represent functional areas (sales, support, legal, security, etc.).

→ [See detailed role definitions](octoacme-roles-and-personas.md)

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- Risk Register
- Retrospective notes and action items

## Lifecycle (high-level)
1. **Initiation**: problem statement, stakeholders, high-level timeline → [Learn more](octoacme-project-initiation.md)
2. **Planning**: scope, resources, milestones, dependencies → [Learn more](octoacme-project-planning.md)
3. **Execution**: build, test, review, iterate → [Learn more](octoacme-execution-and-tracking.md)
4. **Release**: deploy, verify, announce → [Learn more](octoacme-release-and-deployment.md)
5. **Close & Retrospective**: capture learnings and next steps → [Learn more](octoacme-retrospective-and-continuous-improvement.md)

## Communication Cadence
- Weekly sync between PM + PdM
- Twice-weekly standups for delivery team (or as agreed)
- Monthly stakeholder updates
- Ad-hoc escalations as needed

## How to use these docs
- Keep the Project Charter updated in the project repo (in `docs/` folder).
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as institutional knowledge context.
- Use GitHub Issues, Projects, and PRs as the system of record for tracking work.
- For proposing changes to these process docs, use the [issue template](.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml).

## GitHub & Copilot Spaces Integration
- **GitHub Projects**: Use as the primary project board (Backlog → Ready → In Progress → Review → QA → Done)
- **GitHub Issues**: Track all work items, bugs, and decisions with clear labels and acceptance criteria
- **Pull Requests**: Link to issues, include acceptance criteria, and require CI checks before merge
- **Docs Folder**: Keep all process docs and project artifacts in `docs/` for easy discovery
- **Copilot Spaces**: Copy relevant process docs to `.copilot/` to provide context for AI-assisted work
- **Keep Synchronized**: When updating process docs in `docs/`, also update `.copilot/` if those docs are referenced there

## Related Resources
- [Roles and Personas](octoacme-roles-and-personas.md) — Detailed role definitions and interaction points
- [Risk Management & Communication](octoacme-risks-and-communication.md) — Risk practices and escalation paths
- [README](README.md) — Comprehensive guide to all OctoAcme processes
