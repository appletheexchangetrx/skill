# Architecture

## Orchestration
`SKILL.md` is the entry point and workflow orchestrator. It loads only the relevant reference guides for the current task.

## Logical components
- **GitHub discovery:** repository, branch, metadata, tree, file, commit, PR, and workflow inspection.
- **Framework adapter:** React + Vite rules in v1.0; future frameworks add separate adapters.
- **Audit engine:** inventory, comprehensive checks, deep module review, evidence and findings.
- **Coverage ledger:** per-path/module state and exclusion/inaccessibility reasons.
- **Integration adapters:** generic API detection and optional Supabase connector audit.
- **Planning and approval:** findings grouped into user-approved work packages.
- **Development workflow:** branch, implementation, verification, diff review, PR.
- **Reporting:** historical and latest reports in the audited application repository.
- **Readiness evaluator:** weighted score plus mandatory release gates.

## Design constraints
1. Read-only by default.
2. Explicit approval before every class of mutating operation.
3. Evidence and coverage accompany every audit conclusion.
4. Secrets never enter reports, commits, or user-visible output.
5. Framework-specific checks remain isolated.
6. Tool capabilities and permissions must be verified at runtime; never assume an action exists.
