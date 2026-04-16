# Directus

> The flexible backend for all your projects — turn your DB into a headless CMS, admin panels, or apps with a custom UI, instant APIs, auth & more.

| Metric | Data |
|--------|------|
| GitHub | [directus/directus](https://github.com/directus/directus) |
| Stars | 34,802 |
| License | BSL-1.1 (source-available) |
| Language | TypeScript |
| Last Updated | 2026-04-16 |
| Contributors | 500+ |
| Founded | 2012 (13 years) |

## TEMC Score

| Dimension | Score | Rationale |
|-----------|-------|-----------|
| T Technical | 82 | Mature, battle-tested (13 years). Supports any SQL database (Postgres, MySQL, MariaDB, MSSQL, SQLite). REST + GraphQL auto-generated. Vue.js admin. |
| E Ecosystem | 82 | 34.8k stars, 500+ contributors, extensive marketplace of extensions. Strong enterprise adoption. Directus Cloud available. |
| M Market | 78 | Crowded headless CMS space. Directus differentiates as "database-first" — wraps ANY existing DB. But BSL license limits commercial use. |
| C Combination | 72 | Vue.js admin doesn't match base stack (React/Next.js). Backend is Node.js/TypeScript which aligns. Good as API layer but frontend mismatch. |
| **Composite** | **78.2** | T×0.25 + E×0.20 + M×0.25 + C×0.25 |

## Core Value

Directus takes a fundamentally different approach: **database-first**. Instead of defining models in code, you point Directus at any existing SQL database and it auto-generates:
- REST + GraphQL APIs
- Admin panel with RBAC
- File storage
- Authentication
- Webhooks & automation flows

## Architecture Highlights

- **Database agnostic**: Works with existing PostgreSQL, MySQL, MariaDB, MSSQL, SQLite databases
- **Vue.js admin**: Fully customizable data studio
- **Flows engine**: Built-in automation (trigger → condition → action)
- **Extensions**: Custom endpoints, hooks, interfaces, displays, modules
- **Monorepo**: pnpm workspaces, Node 22

## Key Modules for Extraction

1. **Database introspection** — auto-schema detection patterns
2. **RBAC system** — granular role-based access control
3. **Flows engine** — visual automation builder patterns
4. **File storage** — multi-provider abstraction layer
5. **Webhooks** — event-driven notification patterns

## Solo Dev Verdict

🟡 **Good for API-first backends, but license is a concern**. BSL-1.1 means you can self-host but cannot offer Directus as a hosted service. If you need to wrap an existing database with instant APIs + admin panel, Directus is excellent. But for a greenfield SaaS, Payload (MIT, Next.js-native) is a better fit for the base stack. Use Directus when you need to build admin panels on top of existing databases quickly.

---
*Analyzed: 2026-04-16 | TEMC scoring by 天工·内阁首辅*
