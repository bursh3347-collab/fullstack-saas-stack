# Full-Stack SaaS Boilerplate Comparison

> Horizontal comparison of the top full-stack SaaS projects analyzed in this repository.

## Quick Comparison Table

| Project | Stars | Tech Stack | Auth | Payments | Multi-tenant | i18n | TEMC | Best For |
|---------|-------|-----------|------|----------|-------------|------|------|----------|
| **FastAPI Full-Stack** | 42.6k | Python+React+Docker | JWT | ❌ | ❌ | ❌ | 80.3 | Python API-heavy apps |
| **Open SaaS (Wasp)** | 14.1k | Wasp+React+Node | Multi-provider | Stripe+Polar | ❌ | ❌ | 79.6 | Free all-in-one SaaS |
| **SaaS-Boilerplate (ixartz)** | 7.0k | Next.js+Shadcn+TS | Multi-provider | ✅ | ✅ | ✅ | **84.9** | Enterprise Next.js SaaS |
| **Bulletproof React** | 34.8k | React+TS (guide) | Patterns | — | — | — | 82.4 | Architecture reference |
| **SaaS Starter Kit (BoxyHQ)** | 4.8k | Next.js+Tailwind | SSO+SAML | ❌ | ✅ | ❌ | 78.4 | Enterprise SSO/Audit |

## Tech Stack Alignment with Base Stack

> Base stack: TypeScript + Next.js 14 + Tailwind/Shadcn + Supabase + Stripe + Vercel

| Project | Next.js | TypeScript | Tailwind | Shadcn | Stripe | Alignment |
|---------|---------|-----------|----------|--------|--------|----------|
| FastAPI Full-Stack | ❌ React+Vite | ✅ | ❌ Chakra | ❌ | ❌ | 🟡 Low |
| Open SaaS | ❌ Wasp | ✅ | ✅ | ✅ | ✅ | 🟡 Medium (Wasp lock-in) |
| **SaaS-Boilerplate** | **✅** | **✅** | **✅** | **✅** | **✅** | **🟢 Highest** |
| Bulletproof React | ❌ React SPA | ✅ | — | — | — | 🟡 Medium (patterns only) |
| SaaS Starter Kit | ✅ (Pages Router) | ✅ | ✅ | ❌ | ❌ | 🟡 Medium |

## Feature Matrix

| Feature | FastAPI | Open SaaS | ixartz | Bulletproof | BoxyHQ |
|---------|---------|-----------|--------|------------|--------|
| Authentication | JWT | Multi-provider | Multi-provider | Patterns | SSO/SAML |
| Payments | ❌ | Stripe+Polar | ✅ | — | ❌ |
| Multi-tenancy | ❌ | ❌ | ✅ | — | ✅ |
| i18n | ❌ | ❌ | ✅ | — | ❌ |
| Background Jobs | ❌ | ✅ | ❌ | — | ❌ |
| File Upload | ❌ | S3 | ❌ | — | ❌ |
| Email | ❌ | ✅ | ✅ | — | ❌ |
| Audit Logs | ❌ | ❌ | ❌ | — | ✅ |
| SSO/SAML | ❌ | ❌ | ❌ | — | ✅ |
| Docker | ✅ | ❌ | ❌ | — | ❌ |
| CI/CD | ✅ | ❌ | ✅ | — | ❌ |
| Testing | ✅ | ❌ | ✅ | ✅ | ❌ |

## Recommendations

### For One-Person Company (Base Stack Match)
**Winner: ixartz/SaaS-Boilerplate** (TEMC 84.9)
- Perfect tech stack alignment
- Multi-tenancy + i18n = enterprise-ready from day one
- Only 3 open issues = excellent maintenance

### For Architecture Learning
**Winner: Bulletproof React** (TEMC 82.4)
- The React architecture bible
- Feature-based folder structure is industry standard

### For Python Developers
**Winner: FastAPI Full-Stack** (TEMC 80.3)
- Official FastAPI template
- Production Docker setup included

### For Maximum Features (Free)
**Winner: Open SaaS** (TEMC 79.6)
- Most complete free SaaS template
- But Wasp framework lock-in is a concern

### For Enterprise Sales
**Winner: BoxyHQ SaaS Starter Kit** (TEMC 78.4)
- SSO + Audit Logs = enterprise upsell
- But smaller community
