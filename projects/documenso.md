# Documenso

> The Open Source DocuSign Alternative — beautiful, fast, and compliant document signing.

| Metric | Data |
|--------|------|
| GitHub | [documenso/documenso](https://github.com/documenso/documenso) |
| Stars | 12,666 |
| License | AGPL-3.0 |
| Language | TypeScript |
| Last Updated | 2026-04-16 |
| Version | v2.8.1 |
| Contributors | 200+ |

## TEMC Score

| Dimension | Score | Rationale |
|-----------|-------|-----------|
| T Technical | 80 | Remix (migrated from Next.js) + Prisma + tRPC + Tailwind. PDF handling with @libpdf/core + pdfjs-dist. AI integration (Vercel AI SDK + Google Vertex). Inngest for background jobs. |
| E Ecosystem | 72 | 12.7k stars, growing community. Not as large as Cal.com but dedicated. DocuSign/HelloSign alternative niche. |
| M Market | 78 | E-signature market is $7B+. DocuSign dominates but expensive ($10-25/mo per user). Open-source alternative has clear demand. PAdES compliance. |
| C Combination | 75 | TypeScript + Prisma aligns. Remix (not Next.js) is a slight mismatch. Inngest for background jobs is elegant. Stripe integration. PDF expertise is specialized. |
| **Composite** | **76.7** | T×0.25 + E×0.20 + M×0.25 + C×0.25 |

## Core Value

Documenso proves you can build a **production-grade SaaS** as an open-source project:
- Digital signature with PAdES compliance
- Template management
- Team workspaces
- API for programmatic signing
- Self-hostable with Docker
- Revenue model: hosted version + enterprise features

## Architecture Highlights

- **Monorepo**: apps/remix (main app) + apps/docs + packages/*
- **Stack**: Remix + Prisma + PostgreSQL + tRPC
- **Background jobs**: Inngest for async workflows
- **AI**: Vercel AI SDK + Google Vertex for document intelligence
- **PDF**: Custom PDF rendering and signing with @libpdf/core
- **i18n**: Lingui for translations
- **Auth**: Custom auth with Turnstile CAPTCHA
- **Payments**: Stripe integration
- **Analytics**: PostHog + Segment

## Key Modules for Extraction

1. **PDF signing pipeline** — digital signature implementation patterns
2. **Template system** — reusable document template architecture
3. **Inngest integration** — event-driven background job patterns (code-base/automation/)
4. **tRPC + Prisma** — type-safe API layer (similar to Cal.com)
5. **Webhook system** — external integration notifications

## Solo Dev Verdict

🟡 **Excellent case study for building a SaaS business on open-source**. Documenso shows how to: (1) pick a clear incumbent to disrupt (DocuSign), (2) offer self-hosted + cloud, (3) build in public. The Remix migration from Next.js is worth studying for framework choice decisions. **For solo dev**: the e-signature niche requires legal compliance knowledge (PAdES, eIDAS). Better as architecture reference than as a base to fork (AGPL).

---
*Analyzed: 2026-04-16 | TEMC scoring by 天工·内阁首辅*
