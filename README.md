# Web Development & Production Readiness Skill

A GitHub-integrated assistant for auditing, planning, developing, testing, and assessing web applications for production readiness.

**Initial framework scope:** React + Vite  
**Skill specification:** [v1.0](docs/SPECIFICATION-v1.0.md)  
**Main instructions:** [SKILL.md](SKILL.md)

## Capabilities
- Discover accessible GitHub repositories and branches.
- Inventory and audit a complete repository before deep module audits.
- Track audit coverage and evidence-backed P0–P3 findings.
- Audit integrations, with optional Supabase connector support.
- Ask the user questions based on audit findings.
- Implement only approved work on dedicated branches and submit Pull Requests.
- Assess production readiness using a weighted score and mandatory release gates.

## Safety defaults
Audits are read-only. Repository changes, database changes, production configuration, deployment, report writes, and merges require explicit approval. The Skill never commits directly to `main`.

## Audit reports
Reports are saved in the application repository being audited, not in this Skill repository:
- `docs/audit/history/audit-YYYY-MM-DD.md`
- `docs/audit/production-readiness.md`
- `docs/audit/README.md`

## Documentation
- [Specification](docs/SPECIFICATION-v1.0.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Workflow](docs/WORKFLOW.md)
- [Installation and usage](docs/INSTALLATION.md)
- [Changelog](CHANGELOG.md)

## Status
Initial implementation is prepared on `skill/implementation-v1.0`. The user will independently test the completed Skill; it must not be described as user-tested until then.
