# Cal.com

> Open-source scheduling infrastructure for everyone — the Calendly alternative.

| Metric | Data |
|--------|------|
| GitHub | [calcom/cal.com](https://github.com/calcom/cal.com) |
| Stars | ~40,000 |
| License | AGPL-3.0 (+ commercial) |
| Language | TypeScript |
| Last Updated | 2026-04-16 |
| Contributors | 800+ |
| Funding | $32M+ raised |

## TEMC Score

| Dimension | Score | Rationale |
|-----------|-------|-----------|
| T Technical | 90 | Massive monorepo (yarn workspaces + Turborepo). Next.js + Prisma + tRPC. Biome formatter. Playwright E2E. Cal Atoms embeddable components. AI module. |
| E Ecosystem | 88 | 40k stars, 800+ contributors, App Store with 100+ integrations (Google, Zoom, Stripe, Salesforce). Cal.com Platform for white-label. |
| M Market | 85 | Scheduling SaaS is $500M+ market. Cal.com is the clear open-source leader vs Calendly ($3B valuation). Enterprise + self-hosted + platform play. |
| C Combination | 82 | TypeScript + Next.js + Prisma aligns well. Stripe integration. But monorepo is massive (complex for extraction). AGPL limits commercial forking. |
| **Composite** | **86.3** | T×0.25 + E×0.20 + M×0.25 + C×0.25 |

## Core Value

Cal.com is the **most complete open-source scheduling platform** in existence:
- Event types with custom fields, workflows, and routing
- Team scheduling with round-robin and collective availability
- Embeddable booking widgets (Cal Atoms)
- 100+ app integrations
- Cal.com Platform: white-label scheduling API

## Architecture Highlights

- **Monorepo**: apps/web (main app) + apps/api + packages/* (features, platform, embeds, app-store)
- **Stack**: Next.js + Prisma + tRPC + Tailwind + Radix UI
- **App Store**: Plugin architecture for calendar/video/payment integrations
- **Cal Atoms**: React components for embedding scheduling into any app
- **AI module**: `@calcom/ai` for AI-powered scheduling
- **MCP**: `@modelcontextprotocol/sdk` integration in dependencies
- **i18n**: Crowdin-based translation
- **Testing**: Vitest + Playwright

## Key Modules for Extraction

1. **App Store architecture** — plugin system for integrations (pattern reusable for any SaaS)
2. **Embeddable widgets** (Cal Atoms) — React component embedding pattern
3. **Availability engine** — complex scheduling logic
4. **tRPC API layer** — type-safe API patterns
5. **Workflow automation** — event-driven actions (Trigger.dev integration)

## Solo Dev Verdict

🟢 **The gold standard for open-source SaaS architecture**. Even if you're not building scheduling, Cal.com's monorepo structure, App Store plugin system, and embeddable component pattern are worth studying. The tRPC + Prisma + Next.js stack is a masterclass in TypeScript full-stack design. **Caveat**: AGPL-3.0 means you cannot fork and sell as closed-source SaaS — but you can learn from the architecture and reimplement patterns.

---
*Analyzed: 2026-04-16 | TEMC scoring by 天工·内阁首辅*
