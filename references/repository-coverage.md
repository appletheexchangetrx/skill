# Repository Coverage Ledger

Maintain a ledger with path/module, category, status, reason, evidence/reference, and next action.

Allowed statuses:
- Audited
- Partially Audited
- Pending
- Excluded
- Inaccessible

## Rules
- Inventory the complete tree before deep audit.
- Track files individually or in coherent, named groups where the inventory is very large.
- Generated artifacts, dependencies, caches, and build outputs may be Excluded with a clear reason; retain relevant configuration and lockfiles for review.
- A directory listing is not equivalent to source review.
- A file fetched but not analyzed is not Audited.
- Retrieval failure or truncation is Inaccessible/Partially Audited, not Passed.
- Report counts and percentage by status, along with the denominator and exclusions.
- Resume from Pending/Partially Audited items on later sessions using the saved ledger where available.
