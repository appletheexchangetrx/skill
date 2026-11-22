# API and Integration Audit

Discover API endpoints, clients, SDKs, webhooks, auth providers, payment services, analytics, databases, and other external systems from imports, configuration names, environment references, and call sites.

For each integration map:
- Purpose and owner/module.
- Configuration inputs (names only; never values of secrets).
- Authentication method and trust boundary.
- Request/response and error handling.
- Timeout, retry, rate-limit, and validation behavior.
- Data sensitivity and logging.
- Tests, mocks, and operational dependencies.

Do not call live endpoints or mutate external services without user approval. Report connector/access limitations.
