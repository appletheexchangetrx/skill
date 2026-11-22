# Security Audit

Inspect secret exposure, environment handling, authentication and authorization boundaries, client/server trust, input validation, output encoding, dependency advisories, unsafe DOM use, CORS assumptions, storage of tokens, security headers, and sensitive logging.

Never reveal secret values. Report variable names, file paths, and safe redacted evidence. Treat all frontend code and Vite-exposed variables as public. Never place Supabase service-role or other privileged secrets in browser bundles.

Static inspection is not a penetration test. Label unperformed dynamic/security tests Not Run or Not Verified.
