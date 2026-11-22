# Repository Discovery

1. List repositories accessible through the connected GitHub integration.
2. Present useful metadata: owner/name, visibility, default branch, archived state, and permissions when available.
3. Let the user select a repository; do not infer the target from account identity.
4. Retrieve branches and let the user select a branch.
5. Inspect repository metadata and available protection/ruleset information.
6. Record commit/ref used as the audit baseline.
7. If repository is empty, explain that branch-based work requires a bootstrap commit; request explicit one-time approval before initializing the default branch.
