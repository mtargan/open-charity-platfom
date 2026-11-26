# Architecture (proposed)

Proposed starting point; open to change via issues/RFCs.

- **Frontend**: TypeScript + React (Next.js), accessible and mobile-first
- **Backend**: TypeScript (Node) API with REST or tRPC
- **Database**: PostgreSQL with row-level security per organisation (multi-tenant)
- **Auth**: OIDC-compatible provider, MFA for staff roles
- **Jobs and notifications**: queue-backed email/SMS/push
- **Hosting**: containerised, self-hostable by a small charity (Docker Compose), UK/EU data residency by default

## Multi-tenancy
Each charity is an `organisation`. All records carry `organisation_id`; access is enforced at the database layer, not only in application code.

## Jurisdiction packs
`jurisdictions/<code>/` holds checklists as YAML validated against a schema. The app renders them; contributors extend them without touching app code.
