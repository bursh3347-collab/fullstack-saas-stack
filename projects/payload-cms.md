# Payload CMS

> The open-source, fullstack Next.js framework — instant backend superpowers with TypeScript.

| Metric | Data |
|--------|------|
| GitHub | [payloadcms/payload](https://github.com/payloadcms/payload) |
| Stars | 41,852 |
| License | MIT |
| Language | TypeScript |
| Last Updated | 2026-04-16 |
| Contributors | 900+ |
| Version | v3.83.0 |

## TEMC Score

| Dimension | Score | Rationale |
|-----------|-------|-----------|
| T Technical | 88 | Production-grade Next.js native CMS. Monorepo (pnpm+turbo). Supports MongoDB, Postgres, SQLite, Vercel Postgres, D1. Lexical rich text editor. Full TypeScript. |
| E Ecosystem | 85 | 41.8k stars, 900+ contributors, rich plugin ecosystem (ecommerce, form-builder, multi-tenant, SEO, Stripe, MCP, cloud storage). Active Discord. |
| M Market | 80 | Headless CMS market competitive (Strapi, Sanity, Contentful). But Payload's Next.js-native approach is unique differentiator. Growing enterprise adoption. |
| C Combination | 90 | **Perfect base stack match**: Next.js + TypeScript + Tailwind. Built-in auth, file upload, access control, REST+GraphQL API. Plugin for Stripe, multi-tenant, email. |
| **Composite** | **85.1** | T×0.25 + E×0.20 + M×0.25 + C×0.25 |

## Core Value

Payload v3 is a **Next.js-native CMS** — your admin panel IS your Next.js app. No separate backend server. This means:
- One codebase, one deployment (Vercel-ready)
- Full TypeScript end-to-end
- Access control at the field level
- Auto-generated REST + GraphQL APIs
- Live Preview for content editors

## Architecture Highlights

- **Monorepo**: packages/* contains core, UI, database adapters, plugins
- **Database adapters**: MongoDB, Postgres, SQLite, Vercel Postgres, D1 (Cloudflare)
- **Rich text**: Lexical editor with full customization
- **Plugin system**: Modular — ecommerce, form-builder, SEO, redirects, search, Stripe, cloud storage (S3/GCS/R2/Azure/Vercel Blob)
- **MCP plugin**: `@payloadcms/plugin-mcp` — AI-ready CMS!

## Key Modules for Extraction

1. **Auth system** — JWT + session-based, field-level access control, multi-provider
2. **Multi-tenant plugin** — tenant isolation patterns, perfect for SaaS
3. **Stripe plugin** — subscription/payment integration patterns
4. **File upload** — S3/R2/GCS adapters with image optimization
5. **Email** — Nodemailer + Resend adapters

## Solo Dev Verdict

🟢 **Strong pick for content-heavy SaaS**. If your SaaS needs a CMS backend (blog, documentation, landing pages, or content management), Payload v3 is the best open-source option in the Next.js ecosystem. MIT license = zero risk. The multi-tenant + Stripe plugins mean you can build a SaaS in days, not weeks. Main caveat: learning curve for Payload's config-as-code approach.

---
*Analyzed: 2026-04-16 | TEMC scoring by 天工·内阁首辅*
