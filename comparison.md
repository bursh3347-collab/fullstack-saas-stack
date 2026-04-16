# Full-Stack SaaS Boilerplate Comparison

> Horizontal comparison of the top full-stack SaaS projects analyzed in this repository.

## Quick Comparison Table

| Project | Stars | Tech Stack | Auth | Payments | Multi-tenant | i18n | TEMC | Best For |
|---------|-------|-----------|------|----------|-------------|------|------|----------|
| **Supabase (as Base)** | 100.9k | Postgres+TS+Deno | 50+ providers | Stripe webhook | ✅ RLS | ❌ | **93.8** | THE SaaS foundation |
| **Cal.com** | ~40k | Next.js+Prisma+tRPC | Multi-provider | Stripe | ✅ Teams | ✅ | **86.3** | SaaS architecture reference |
| **Payload CMS** | 41.9k | Next.js native CMS | Built-in | Stripe plugin | ✅ Plugin | ❌ | **85.1** | Content-heavy SaaS |
| **SaaS-Boilerplate (ixartz)** | 7.0k | Next.js+Shadcn+TS | Multi-provider | ✅ | ✅ | ✅ | **84.9** | Enterprise Next.js SaaS |
| **Bulletproof React** | 34.8k | React+TS (guide) | Patterns | — | — | — | 82.4 | Architecture reference |
| **FastAPI Full-Stack** | 42.6k | Python+React+Docker | JWT | ❌ | ❌ | ❌ | 80.3 | Python API-heavy apps |
| **Open SaaS (Wasp)** | 14.1k | Wasp+React+Node | Multi-provider | Stripe+Polar | ❌ | ❌ | 79.6 | Free all-in-one SaaS |
| **SaaS Starter Kit (BoxyHQ)** | 4.8k | Next.js+Tailwind | SSO+SAML | ❌ | ✅ | ❌ | 78.4 | Enterprise SSO/Audit |
| **Directus** | 34.8k | Node+Vue.js | Built-in RBAC | ❌ | ❌ | ✅ | **78.2** | Database-first admin |
| **Documenso** | 12.7k | Remix+Prisma+tRPC | Custom | Stripe | ✅ Teams | ✅ | **76.7** | OSS SaaS business model |

## Tech Stack Alignment with Base Stack

> Base stack: TypeScript + Next.js 14 + Tailwind/Shadcn + Supabase + Stripe + Vercel

| Project | Next.js | TypeScript | Tailwind | Shadcn | Stripe | Alignment |
|---------|---------|-----------|----------|--------|--------|----------|
| Supabase (as Base) | ✅ template | ✅ | ✅ | ✅ | ✅ webhook | 🟢 **Perfect** |
| Cal.com | ✅ | ✅ | ✅ | ❌ Radix | ✅ | 🟢 High |
| **Payload CMS** | **✅ native** | **✅** | **✅** | ❌ Radix | **✅ plugin** | **🟢 High** |
| **SaaS-Boilerplate** | **✅** | **✅** | **✅** | **✅** | **✅** | **🟢 Highest** |
| Bulletproof React | ❌ React SPA | ✅ | — | — | — | 🟡 Medium |
| FastAPI Full-Stack | ❌ React+Vite | ✅ | ❌ Chakra | ❌ | ❌ | 🟡 Low |
| Open SaaS | ❌ Wasp | ✅ | ✅ | ✅ | ✅ | 🟡 Medium (Wasp lock-in) |
| SaaS Starter Kit | ✅ (Pages) | ✅ | ✅ | ❌ | ❌ | 🟡 Medium |
| **Directus** | ❌ Vue.js | ✅ | ❌ | ❌ | ❌ | 🔴 Low |
| **Documenso** | ❌ Remix | ✅ | ✅ | ❌ | ✅ | 🟡 Medium |

## License Risk Matrix

| Project | License | Commercial SaaS | Fork & Sell | Risk |
|---------|---------|----------------|-------------|------|
| Supabase | Apache-2.0 | ✅ | ✅ | 🟢 Low |
| Payload CMS | MIT | ✅ | ✅ | 🟢 Low |
| Bulletproof React | MIT | ✅ | ✅ | 🟢 Low |
| FastAPI Full-Stack | MIT | ✅ | ✅ | 🟢 Low |
| SaaS-Boilerplate | MIT | ✅ | ✅ | 🟢 Low |
| Open SaaS | MIT | ✅ | ✅ | 🟢 Low |
| SaaS Starter Kit | Apache-2.0 | ✅ | ✅ | 🟢 Low |
| Directus | BSL-1.1 | ⚠️ No competing | ⚠️ | 🟡 Medium |
| Cal.com | AGPL-3.0 | ❌ Must open-source | ❌ | 🔴 High |
| Documenso | AGPL-3.0 | ❌ Must open-source | ❌ | 🔴 High |

## Recommendations

### For One-Person Company (Base Stack Match)
**Winner: Supabase + ixartz/SaaS-Boilerplate + Payload CMS**
- Supabase as backend foundation
- ixartz for SaaS boilerplate (perfect alignment, TEMC 84.9)
- Payload CMS if content management needed

### For SaaS Architecture Learning
**Winner: Cal.com** (TEMC 86.3)
- The most complete open-source SaaS codebase
- App Store plugin pattern, embeddable components, tRPC+Prisma

### For OSS SaaS Business Model Study
**Winner: Documenso** (TEMC 76.7)
- Shows how to build a business on AGPL + commercial license

### For Database-First Admin Panels
**Winner: Directus** (TEMC 78.2)
- Point at any SQL database, get instant APIs + admin panel

---
*Last updated: 2026-04-16 | TEMC scoring by 天工·内阁首辅*
