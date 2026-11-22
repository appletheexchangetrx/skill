# GitHub Integration

## Discovery
Use the connected GitHub tools to list accessible repositories and branches dynamically. Do not hardcode repository names. Verify repository identity, default branch, visibility, archive state, and granted permissions.

## Read operations
Inspect repository tree recursively where supported, then fetch relevant files by exact path and selected ref. Read manifests, lockfiles, source, tests, configuration, workflows, deployment files, migrations, and documentation. Paginate or continue retrieval where the tool supports it. Record inaccessible or truncated results.

## Write operations
Only after explicit approval:
1. Confirm repository, base branch, and exact scope.
2. Create a descriptive branch from the selected base.
3. Apply only approved changes on that branch.
4. Fetch/review the resulting files and diff.
5. Run available checks or clearly mark them Not Run.
6. Create a PR with scope, test results, risks, and remaining work.
Never update main directly or merge without explicit approval.

## Limits
Connector capabilities vary. Check available actions and permissions at runtime. Do not claim local execution, browser testing, CI status, branch protection, or workflow results unless actually obtained.
