# Example Audit Report (Illustrative Only)

> Fictional sample content to demonstrate format. This is not an actual repository audit.

- Repository: `example/storefront`
- Branch: `main`
- Mode: Repository Only
- Coverage: 42 audited, 3 excluded, 0 pending, 0 inaccessible

## Executive summary
The illustrative application builds, but one high-priority authorization concern and an unverified deployment configuration prevent a Production Ready conclusion.

## Example finding
| ID | Priority | Module | Finding | Evidence | Recommendation | Status |
|---|---|---|---|---|---|---|
| EX-001 | P1 | API client | Client assumes protected resource access is enforced by UI | Illustrative call site in `src/services/example.ts` | Verify server-side authorization and add negative tests | Open |

## Example verification
| Check | Status |
|---|---|
| Build | Passed |
| Unit tests | Not Run |
| Deployment verification | Not Verified |

## Example readiness
**Not Confirmed** — illustrative score 86/100 does not override the unverified deployment gate.
