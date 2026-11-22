# React + Vite Audit

Inspect:
- `package.json`, lockfile, Node/package manager expectations.
- Vite config, plugins, base path, aliases, dev-server exposure, build output.
- React entry point, root rendering, StrictMode, routing strategy.
- Component boundaries, hooks, context/state, data fetching, error/loading/empty states.
- TypeScript configuration and type safety where used.
- CSS strategy, Tailwind configuration/plugins, design tokens, responsive breakpoints.
- Asset handling, lazy loading, route/component splitting.
- Environment variable conventions and client-exposed variables.
- Build, preview, test, lint, and type-check scripts.
- SPA fallback and hosting configuration for client-side routes.

Do not assume a missing test/lint script is a defect without assessing project risk and context. Recommend proportionate checks.
