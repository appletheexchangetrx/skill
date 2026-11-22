# Web Development & Production Readiness Skill — Specification v1.0

**Status:** Approved implementation baseline  
**Initial framework:** React + Vite  
**Platform:** GitHub through the connected GitHub integration; optional Supabase through the connected Supabase integration.

## Objective
Help users audit, plan, develop, test, document, and assess web applications for production readiness. The Skill proactively identifies evidence-backed improvements and asks the user before implementing them.

## Scope
Initial support covers React, Vite, JavaScript, TypeScript, HTML, CSS, and Tailwind CSS. Framework adapters must remain modular for later Next.js, Vue, Nuxt, Angular, and other support.

## GitHub
Dynamically discover accessible repositories and branches; inspect metadata, files, commits, CI/CD, and protections where available. Never commit directly to `main`. Implement approved work on a dedicated branch and submit a Pull Request. User approval is required before merge.

## Audit sequence
1. Repository and branch selection.
2. Stack/integration detection and Supabase mode selection.
3. Full repository inventory.
4. Comprehensive audit of all relevant files.
5. Deep audit per module.
6. Consolidated assessment, priorities, questions, and plan.

Coverage states: Audited, Partially Audited, Pending, Excluded, Inaccessible. Exclusions require reasons. Incomplete coverage must be disclosed.

## Audit domains
Project health, architecture, code quality, dependencies, UI/UX, responsive design, performance, security, SEO, accessibility, APIs, database, authentication, external integrations, deployment, CI/CD, and monitoring.

## Supabase optional mode
Repository Only must work without Supabase. Repository + Supabase detects the project configuration, matches it to projects accessible through the connected integration, and asks for confirmation before inspection. Audit is read-only by default. Missing access is reported as Not Verified/Inaccessible. Never expose secrets or place service-role credentials in frontend code.

## Reporting
After user approval, save reports in the audited application repository:
- `docs/audit/history/audit-YYYY-MM-DD.md`
- `docs/audit/production-readiness.md`
- `docs/audit/README.md`

Each approved audit creates a new historical report and refreshes the latest report. Preserve history and compare findings as New, Open, Resolved, or Reopened.

## Priorities
P0 Critical, P1 High, P2 Medium, P3 Low. Each finding requires evidence, affected paths, impact, recommendation, and verification.

## Approval and development
Ask finding-based questions; group work; prepare affected-file plan and acceptance criteria; obtain approval before changes. Separate approval is required for repository changes, database changes, production configuration, deployment, and merge. Test, inspect diffs, then open a PR. Never merge without explicit user approval.

## Production readiness
Minimum 85/100, no open P0/P1, all critical security checks passed, production build passed, core journeys and relevant integrations verified, and deployment/configuration verified. Unknown checks are Not Verified, not Passed. N/A weights require transparent redistribution. Without sufficient evidence, readiness is Not Confirmed.

## User testing
The user performs independent testing after Skill completion. Do not describe the Skill as user-tested before that occurs.
