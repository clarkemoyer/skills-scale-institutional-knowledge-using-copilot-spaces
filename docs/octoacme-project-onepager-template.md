# OctoAcme — Project One-pager Template

**Navigation**: [Overview](octoacme-project-management-overview.md) | [Initiation](octoacme-project-initiation.md)

## Purpose
This template provides a structured format for creating a Project One-pager (also called a Project Charter) during the initiation phase. A well-crafted one-pager aligns stakeholders, clarifies the problem and goals, and serves as the foundation for planning.

## When to Use
- During project initiation, after initial discovery and before detailed planning
- When proposing a new project or feature for stakeholder approval
- As a reference document throughout the project lifecycle

## Instructions
1. Copy this template into your project repository (`docs/project-onepager.md`)
2. Fill in all sections with clear, concise information
3. Review with Product Manager and key stakeholders
4. Use as input for planning kickoff and backlog creation
5. Keep updated as the project evolves

---

## Project One-pager: [Project Name]

### Project Overview
**Project Name**: [Descriptive name of the project]

**Last Updated**: [Date]

**Status**: [Draft | In Planning | In Execution | Released | Closed]

### Problem Statement
[Describe the problem you're solving in 2-3 sentences. Be specific about who is affected and what pain points exist.]

**Example**: "Customer support teams are spending 40% of their time manually categorizing support tickets, leading to slow response times and frustrated customers. There is no automated system to route tickets to the appropriate team based on content and urgency."

### Objective / Goal
[State what success looks like. Use SMART criteria: Specific, Measurable, Achievable, Relevant, Time-bound.]

**Example**: "Implement an automated ticket categorization and routing system that reduces manual categorization time by 70% and improves average first-response time from 4 hours to 1 hour within 6 months of deployment."

### Success Metrics
[Define 3-5 measurable outcomes that indicate project success]

- **Metric 1**: [e.g., Reduce manual ticket categorization time by 70%]
- **Metric 2**: [e.g., Improve first-response time from 4h to 1h]
- **Metric 3**: [e.g., Achieve 90% categorization accuracy]
- **Metric 4**: [e.g., Support team satisfaction score improves from 6/10 to 8/10]
- **Metric 5**: [e.g., Zero increase in infrastructure costs]

**Measurement Plan**: [How and when will you measure these metrics?]

### Target Users / Customers
[Who will benefit from this project?]

- **Primary**: [e.g., Customer support agents, support managers]
- **Secondary**: [e.g., Customers receiving support, product team needing feedback data]

### Stakeholders & Decision Makers

| Name | Role | Responsibility | Contact |
|------|------|----------------|---------|
| [Name] | Sponsor / Executive | Approves go/no-go, provides budget/resources | [email/slack] |
| [Name] | Product Manager | Defines requirements, prioritizes backlog | [email/slack] |
| [Name] | Project Manager | Coordinates delivery, manages timeline | [email/slack] |
| [Name] | Tech Lead | Technical decisions, architecture | [email/slack] |
| [Name] | Support Lead | Subject matter expert, user feedback | [email/slack] |
| [Name] | UX Designer | User experience design | [email/slack] |

### Proposed Timeline & Milestones

| Milestone | Target Date | Description | Exit Criteria |
|-----------|-------------|-------------|---------------|
| **Initiation Complete** | [Date] | Stakeholder alignment, one-pager approved | Sponsor approves, planning kickoff scheduled |
| **Planning Complete** | [Date] | Backlog created, architecture designed | Sprint 1 ready to start, DoD defined |
| **Alpha/MVP** | [Date] | Core functionality working in staging | Key features complete, passes smoke tests |
| **Beta** | [Date] | Feature-complete, ready for pilot users | All acceptance criteria met, pilot users identified |
| **GA Release** | [Date] | Production deployment | Successful deployment, metrics tracked |
| **Retrospective** | [Date] | Lessons learned captured | Retro complete, action items created |

**Total Estimated Duration**: [e.g., 4 months from initiation to GA]

### Scope & Key Features

#### In Scope
- [Feature or capability 1]
- [Feature or capability 2]
- [Feature or capability 3]

#### Out of Scope (for this iteration)
- [Feature or capability to be deferred]
- [Feature or capability to be handled separately]

#### Assumptions
- [Assumption 1, e.g., "Existing ticketing API supports webhook integration"]
- [Assumption 2, e.g., "Support team has capacity for 2-week pilot period"]

### Initial Risk Assessment

| Risk ID | Description | Impact (H/M/L) | Likelihood (H/M/L) | Mitigation Strategy |
|---------|-------------|----------------|-------------------|---------------------|
| RISK-001 | [Risk description] | High | Medium | [What will you do to reduce this risk?] |
| RISK-002 | [Risk description] | Medium | Low | [Mitigation plan] |
| RISK-003 | [Risk description] | High | High | [Mitigation plan + contingency] |

→ [See full Risk Register](octoacme-risks-and-communication.md)

### Dependencies

#### Internal Dependencies
- [Dependency on another team or system, e.g., "Auth service team to provide SSO integration by Sprint 2"]
- [Dependency description]

#### External Dependencies
- [External vendor, API, or service, e.g., "Third-party ML API for text classification"]
- [Dependency description]

**Dependency Tracking**: [Link to GitHub Issues or dependency tracker]

### Resource Requirements

#### Team Composition
- **Project Manager**: [Name or TBD] - [% allocation]
- **Product Manager**: [Name or TBD] - [% allocation]
- **Developers**: [Number] developers - [% allocation]
- **QA Lead**: [Name or TBD] - [% allocation]
- **UX Designer**: [Name or TBD] - [% allocation]
- **Scrum Master**: [Name or TBD] - [% allocation]
- **Business Analyst**: [Name or TBD] - [% allocation] (if needed)

#### Budget
- **Development Costs**: [Estimate]
- **Infrastructure Costs**: [Estimate for cloud resources, services, etc.]
- **Third-party Licenses/APIs**: [Estimate]
- **Total Estimated Budget**: [Total]

### GitHub & Documentation Links

- **GitHub Repository**: [Link to repo]
- **GitHub Project Board**: [Link to project board]
- **Copilot Space**: [Link or instructions to access]
- **Design Docs/Wireframes**: [Link to design files]
- **Technical Architecture**: [Link to architecture doc]
- **Meeting Notes**: [Link to folder or doc]

### Communication Plan

| Audience | Method | Frequency | Owner |
|----------|--------|-----------|-------|
| Delivery Team | Daily standup | Daily | Scrum Master |
| Stakeholders | Email update | Weekly | Project Manager |
| Executives | Dashboard + monthly review | Monthly | Product Manager |
| Support Team | Release notes + training | Per release | Project Manager |

### Approval & Sign-off

| Role | Name | Approval Date | Signature/Notes |
|------|------|---------------|-----------------|
| Sponsor | [Name] | [Date] | [Approved / Conditional / Notes] |
| Product Manager | [Name] | [Date] | [Approved / Conditional / Notes] |
| Tech Lead | [Name] | [Date] | [Approved / Conditional / Notes] |

**Decision**: [Go / No-Go / Conditional Go]

**Next Steps**: [e.g., "Schedule planning kickoff for [date]", "Address budget questions with finance"]

---

## Tips for a Great Project One-pager

### Be Concise
- Keep it to 2-3 pages max (this template is comprehensive but should be filled in concisely)
- Use bullet points, tables, and clear headers
- Link to detailed docs rather than including everything

### Focus on Outcomes
- Emphasize the "why" and "what" more than the "how"
- Define success in measurable terms
- Connect to business or customer value

### Get Stakeholder Input Early
- Share a draft with key stakeholders before finalizing
- Incorporate feedback to ensure alignment
- Use the one-pager as a discussion tool, not just a status doc

### Keep It Updated
- Review and update at each major milestone
- Reflect scope changes, timeline adjustments, or new risks
- Archive old versions to show project evolution

### Link to the Lifecycle
- Use this one-pager as the starting point for planning
- Reference it in status updates to show progress toward goals
- Review it in retrospectives to assess whether goals were achieved

---

## Related Resources
- [Project Initiation Guide](octoacme-project-initiation.md) — How to use this template during initiation
- [Project Planning Guide](octoacme-project-planning.md) — Next steps after one-pager is approved
- [Risk Management & Communication](octoacme-risks-and-communication.md) — Detailed risk and communication practices
- [Roles and Personas](octoacme-roles-and-personas.md) — Understanding stakeholder roles
- [Project Management Overview](octoacme-project-management-overview.md) — Full lifecycle context
