# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
  - Attendees: Developers, QA Lead, Project Manager, and others as needed
  - QA Lead reports on testing status and quality concerns
  - UX/UI Designer joins as needed for design clarifications
- Weekly delivery sync — show progress, updates, and flagged risks
  - Business Analyst validates features meet requirements
  - Release Manager tracks release readiness
- Demo/Review at the end of each sprint or milestone
  - UX/UI Designer validates design implementation
  - Business Analyst confirms business requirements are met
  - QA Lead presents quality metrics and test results

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - UX/UI Designer reviews PRs affecting user interface
  - QA Lead reviews for testability and test coverage
  - Require at least one approval before merging (or team-defined policy)
  - Business Analyst validates functional requirements are met (for significant changes)

## Quality & Testing
- QA Lead oversees all testing activities and quality standards
- Unit tests for new logic (developer-owned, QA Lead reviews coverage)
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed
- Usability testing coordinated by UX/UI Designer for new interfaces
- User Acceptance Testing (UAT) coordinated by Business Analyst with business stakeholders

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] QA Lead has access to test environments and tools
- [ ] UX/UI Designer has access to review builds/staging environments
- [ ] Business Analyst has defined UAT criteria and test scenarios
- [ ] Regular demos scheduled with all relevant stakeholders
- [ ] Risk register updated weekly by Project Manager
- [ ] Quality metrics tracked and reported by QA Lead
