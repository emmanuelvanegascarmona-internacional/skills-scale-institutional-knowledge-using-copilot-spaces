# OctoAcme Project Management Process Documentation

## Overview
OctoAcme follows a structured, phase-based approach to project delivery that emphasizes customer-first thinking, iterative delivery, and clear ownership. Projects move through initiation, planning, execution, release, and continuous improvement. Each phase uses lightweight artifacts—such as a Project One-pager, prioritized backlog, Definition of Done, and a Risk Register—to keep the team aligned, reduce single-person dependency, and make processes discoverable and actionable for all roles.

## Quick summary of core workflows
- Initiation: Capture the problem, objective, success metrics, stakeholders, and initial risks in a Project One-pager. Move to planning only when success metrics and stakeholders are aligned and team availability is confirmed.
- Planning: Run a kickoff, create a prioritized backlog with acceptance criteria, estimate scope, and define the Definition of Done and release milestones.
- Execution & Tracking: Use a project board (Backlog → Ready → In Progress → In Review → QA → Done). Encourage small PRs linked to issues, require automated CI and at least one reviewer approval, and track progress with daily standups and weekly delivery syncs.
- Release & Deployment: Follow pre-release checklists (passing CI/security scans, release notes, rollback plan), run staging smoke tests, and deploy to production via automated pipelines when possible. Use rollback/playbook steps and post-deploy verification as needed.
- Retrospective & Continuous Improvement: Timebox retrospectives after sprints or incidents, prioritize 2–3 action items, and add follow-ups to the backlog for measurable improvement.

## Key personas & responsibilities
- Product Manager (PdM): Defines the problem, outcomes, success metrics, and prioritization.
- Project Manager (PM): Coordinates delivery, schedules, manages risks and communications, and maintains project artifacts.
- Developers: Implement features, write tests, and participate in design and reviews.
- QA/Testing: Validate acceptance criteria, perform manual or automated QA as needed.
- Stakeholders: Provide inputs, approvals, and domain context.

## Communication cadence & escalation
- Daily standups (15 min) for progress, blockers, and dependencies.
- Weekly delivery sync to surface progress, risks, and cross-team dependencies.
- PM + PdM weekly alignment and monthly stakeholder updates.
- Escalation path: Team → PM → Product Lead → Sponsor. For security incidents, follow the security incident runbook and notify Security on-call.

## Quality assurance & release controls
- Unit tests for new logic; integration tests where applicable; end‑to‑end smoke tests for critical flows.
- Security scanning integrated in CI.
- Manual QA for feature acceptance when needed.
- Pre-release checklist: passing CI and security scans, release notes, rollback plan, staging smoke tests, and post-deploy verification.

## Quick links (docs/)
- Project Management Overview — ./octoacme-project-management-overview.md
- Project Initiation — ./octoacme-project-initiation.md
- Project Planning — ./octoacme-project-planning.md
- Execution & Tracking — ./octoacme-execution-and-tracking.md
- Risks & Communication — ./octoacme-risks-and-communication.md
- Release & Deployment — ./octoacme-release-and-deployment.md
- Retrospective & Continuous Improvement — ./octoacme-retrospective-and-continuous-improvement.md
- Roles & Personas — ./octoacme-roles-and-personas.md

## How to use this README
- Use this as the central entry point for process docs in the docs/ folder.
- Link from project READMEs or a repo-level contributing guide to help new team members find the right guidance for each project phase or persona.
