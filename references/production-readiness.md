# Production Readiness Assessment

## Weighted rubric (100 points)
| Category | Weight |
|---|---:|
| Code Quality & Architecture | 15 |
| Security | 20 |
| Functionality & Reliability | 15 |
| Performance | 10 |
| UI/UX & Responsive | 10 |
| Accessibility | 10 |
| SEO | 5 |
| API & Integrations | 10 |
| Deployment & Monitoring | 5 |
| **Total** | **100** |

Score only evidence-backed checks. Explain category scoring and evidence. If a category is Not Applicable, justify it and redistribute its weight proportionally across applicable categories; show the adjusted weights. Do not award full points merely because a check was not run.

## Mandatory gates
Production Ready requires all:
- Score >= 85/100.
- No unresolved P0 or P1 findings.
- All critical security checks Passed.
- Production build Passed.
- Core user journeys verified.
- Relevant integrations verified.
- Deployment and production configuration verified.
- Sufficient audit coverage and evidence.

If a blocker exists, status is Not Ready. If a required check is unverified or coverage is insufficient, status is Not Confirmed. A score >=85 does not override a failed gate.

## Report statuses
- **Production Ready:** all score and mandatory gates pass.
- **Not Ready:** one or more blockers/failing gates.
- **Not Confirmed:** evidence or access is insufficient to decide.

Include score, gate-by-gate result, unresolved findings, Not Verified items, coverage, and next steps.
