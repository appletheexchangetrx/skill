# Optional Supabase Integration

## Modes
- Repository Only: no Supabase connection required.
- Repository + Supabase: use the connected ChatGPT Supabase integration if available and authorized.

## Matching
Detect Supabase project URL/reference from repository configuration. Do not reveal credentials. Compare the project reference with accessible projects returned by the connector. Show the proposed match and ask the user to confirm before querying project metadata or data.

## Read-only audit
Where supported, inspect project configuration, schema, tables, relationships, primary/foreign keys, RLS status and policies, grants/privileges, indexes, query/performance advisories, Auth configuration, Storage buckets/access policies, Edge Functions, API usage, logs, and security advisories.

## Safety
- No schema/data writes, migrations, function deployment, policy changes, or production changes during audit.
- Never request or expose service-role keys.
- Do not put privileged keys in client-side code.
- Avoid dumping personal/customer data. Prefer schema and metadata.
- If a tool cannot inspect a domain, mark it Not Verified/Inaccessible and continue other audit areas.
- Any remediation requiring Supabase writes needs a separate plan and explicit approval.
