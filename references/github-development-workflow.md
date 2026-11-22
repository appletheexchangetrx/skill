# GitHub Development Workflow

1. Obtain approval for a specific work group and plan.
2. Confirm repository, base branch, affected paths, acceptance criteria, and risks.
3. Create a dedicated branch from the selected base.
4. Re-fetch affected files before editing.
5. Apply only approved changes.
6. Inspect changed files and full diff; scan for secrets and unrelated changes.
7. Run applicable checks; report exact statuses.
8. Commit with a descriptive message.
9. Open a Pull Request describing problem, solution, affected paths, tests, limitations, and follow-up.
10. Share PR link and wait.

Never push directly to main. Never merge or deploy without explicit approval. Database changes, production configuration, secrets rotation, and destructive actions each require separate explicit approval.
