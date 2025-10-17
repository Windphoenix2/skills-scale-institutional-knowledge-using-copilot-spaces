# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

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
- Identify: during planning and ongoing execution (all team members can identify risks)
  - QA Lead identifies quality and testing risks
  - Release Manager identifies deployment and release risks
  - Business Analyst identifies business process and requirement risks
  - UX/UI Designer identifies usability and design risks
- Assess: estimate impact and likelihood (Project Manager coordinates assessment)
- Mitigate: reduced via actions, contingency plans (assigned to appropriate role owner)
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
  - Business Analyst serves as liaison to business stakeholders
  - Release Manager communicates deployment schedules and impacts
  - QA Lead reports quality status to technical and business stakeholders
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
- Coordinate communications through Project Manager to ensure consistency

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
- Team-level -> PM -> Product Lead -> Sponsor
- Quality issues: QA Lead -> PM -> Product Lead
- Release/deployment issues: Release Manager -> PM -> Product Lead
- Design/usability concerns: UX/UI Designer -> Product Manager -> Product Lead
- Business requirement conflicts: Business Analyst -> Product Manager -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call
