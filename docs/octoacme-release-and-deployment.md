# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- QA Lead sign-off on quality criteria
- Business Analyst confirms business requirements validated
- UX/UI Designer approves design implementation (if UI changes)
- Release notes drafted (by Product Manager with input from Business Analyst)
- Rollback / mitigation plan documented by Release Manager
- Smoke tests prepared by QA Lead

## Deployment Checklist
- [ ] Release Manager schedules deployment window (if needed)
- [ ] Backup or snapshot completed (if applicable)
- [ ] Deploy to staging environment
- [ ] QA Lead runs smoke tests on staging
- [ ] Business Analyst validates critical business workflows (if applicable)
- [ ] Release Manager authorizes production deployment
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] QA Lead confirms production smoke tests pass
- [ ] Release Manager announces release to stakeholders and support
- [ ] Business Analyst notifies business users of changes

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Release Manager triggers incident response and notifies on-call
  - QA Lead assesses severity and impact
  - Release Manager executes rollback to last known-good release if necessary
  - Project Manager coordinates with stakeholders
  - Business Analyst assesses business impact
  - Triage root cause and capture action items
  - Schedule retrospective to prevent recurrence

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
