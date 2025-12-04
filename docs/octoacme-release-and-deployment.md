# OctoAcme — Release & Deployment Guide

**Navigation**: [← Execution](octoacme-execution-and-tracking.md) | [Overview](octoacme-project-management-overview.md) | [Next: Retrospective →](octoacme-retrospective-and-continuous-improvement.md)

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- **Release name / number**: (e.g., v1.2.0, Sprint 42 Release)
- **Date**: (YYYY-MM-DD)
- **Summary**: Brief overview of what's included
- **Notable changes**:
  - New features (link to GitHub Issues)
  - Bug fixes (link to GitHub Issues)
  - Performance improvements
  - Breaking changes (if any)
- **Migration steps** (if any): Step-by-step instructions for users or operators
- **Known issues**: Document any outstanding bugs or limitations
- **Rollback instructions**: How to revert if needed
- **Contributors**: Thank the team members who contributed

**GitHub Integration**: Create a GitHub Release with these notes, tag the release, and link to all merged PRs and closed issues.

## Role Responsibilities in Release

### Project Manager
- Coordinates release timeline and communication
- Ensures all pre-release requirements are met
- Communicates release status to stakeholders
- Coordinates rollback if needed

### Product Manager
- Approves that release meets acceptance criteria and goals
- Reviews release notes for accuracy and completeness
- Plans release announcement and user communication

### QA Lead
- Executes final regression testing in staging
- Verifies all acceptance criteria are met
- Runs post-deployment smoke tests
- Signs off on release readiness

### Developers
- Ensure all PRs are merged and code is in deployable state
- Prepare deployment scripts or automation
- Monitor deployment and address issues
- Available for rollback or hotfixes if needed

### Scrum Master
- Facilitates release retrospective
- Tracks any process improvements for future releases
- Ensures lessons learned are captured

### Stakeholders
- Review and approve release (if required)
- Prepare their teams for changes (support, sales, etc.)
- Provide feedback post-release

## GitHub Workflow for Releases

### Pre-Release Preparation
1. **Create a release branch** (if using GitFlow): `release/v1.2.0`
2. **Tag the release** in GitHub: Use semantic versioning (v1.2.0)
3. **Create GitHub Release**: Draft release notes with all changes
4. **Link all relevant Issues and PRs**: Ensure traceability from requirement to release
5. **Run CI/CD pipeline**: Verify all tests pass, security scans clear

### Deployment Process
1. **Deploy to staging**: Use GitHub Actions or deployment pipeline
2. **Run smoke tests**: Verify critical paths work in staging
3. **Get approval**: QA Lead and PM approve staging deployment
4. **Deploy to production**: Use automated pipeline when possible
5. **Verify deployment**: Run post-deployment checks and smoke tests
6. **Monitor**: Watch metrics, logs, and alerts for anomalies
7. **Announce release**: Communicate to stakeholders via agreed channels

### Post-Deployment
- [ ] Verify key features are working (smoke tests)
- [ ] Monitor error rates, latency, and user feedback
- [ ] Update status page or internal dashboard
- [ ] Send release announcement to stakeholders
- [ ] Close release milestone in GitHub Project
- [ ] Schedule retrospective (within 1-3 days)

## Decision Gate
Release is approved when:
- All acceptance criteria for milestone are met
- QA Lead has signed off on testing
- Product Manager has approved the release
- Rollback plan is documented and understood
- Stakeholders are notified of deployment window

**Decision Makers**: QA Lead (quality sign-off), Product Manager (approve), Project Manager (coordinate)

## Handoff to Retrospective
After the release is deployed and stable:
- [ ] Schedule retrospective within 1-3 days
- [ ] Gather feedback from team on what went well and what could improve
- [ ] Document any incidents or issues during deployment
- [ ] Prepare metrics (deployment time, issues found, rollback needed?)

→ [Next: Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)

## Related Resources
- [Project Management Overview](octoacme-project-management-overview.md) — Full lifecycle context
- [Roles and Personas](octoacme-roles-and-personas.md) — Who does what during release
- [Risk Management & Communication](octoacme-risks-and-communication.md) — Incident management and escalation
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) — Capturing learnings
