# Repository Audit

## Inventory
Enumerate the complete repository tree. Classify files by module and purpose. Identify manifests, lockfiles, source, tests, assets, environment templates, API clients, migrations, workflows, hosting and deployment configuration.

## Comprehensive checks
Review all relevant files, not only entry points. Follow imports and references to map module relationships. Inspect configuration and scripts. Identify external integrations and data flows. Separate verified findings from inferred risks.

## Evidence format
For each issue record:
- Stable finding ID.
- Priority and category.
- Affected path(s) and symbol/config key.
- Observed evidence (avoid secret values).
- Impact and conditions.
- Recommended remediation.
- Verification method and result.

## Completeness
Track every path/module in the coverage ledger. Explain exclusions, inaccessible files, size limits, and partial retrieval. Full audit completion requires all relevant paths to be Audited or explicitly Excluded with rationale; otherwise report partial coverage.
