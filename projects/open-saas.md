# Open SaaS by Wasp

> A 100% free, modern full-stack SaaS boilerplate with React, Node.js, Prisma, and everything you need to launch.

| Metric | Data |
|------|------|
| GitHub | [wasp-lang/open-saas](https://github.com/wasp-lang/open-saas) |
| Stars | 14,102 |
| Forks | 1,652 |
| License | MIT |
| Language | TypeScript |
| Last Updated | 2026-04-15 |
| Open Issues | 114 |
| Contributors | 80+ |

## TEMC Scores

| Dimension | Score | Reasoning |
|------|------|------|
| T (Tech) | 82 | Built on Wasp framework (DSL for full-stack). React + Node.js + Prisma + PostgreSQL. Good code quality but Wasp adds a learning curve and lock-in. |
| E (Ecosystem) | 78 | 14.1k stars, active community. Wasp framework growing but niche. AI-ready with AGENTS.md and Claude Code plugin. |
| M (Market) | 85 | 100% free (competitors charge $200-500). Full SaaS features: Auth (email/Google/GitHub/Slack/MS), Stripe/Polar.sh payments, email, background jobs, S3 upload. |
| C (Combo) | 70 | Wasp framework creates lock-in — can't easily extract modules to non-Wasp projects. However, patterns and architecture decisions are valuable references. |
| **Overall** | **79.6** | T×0.25 + E×0.20 + M×0.30 + C×0.25 |

## Core Value

The most feature-complete FREE SaaS boilerplate available. Key features:
- **Auth**: Email, Google, GitHub, Slack, Microsoft
- **Payments**: Stripe + Polar.sh integration
- **Email**: Built-in email sending
- **Background Jobs**: Server-side job processing
- **Landing Page**: Pre-built marketing page
- **Admin Dashboard**: Analytics and user management
- **AI-Ready**: Tailored AGENTS.md, skills, Claude Code plugin
- **S3 File Upload**: Built-in file management
- **One-cmd deploy**: Simplified deployment

## Architecture Highlights

Built on Wasp's declarative DSL that compiles to React + Node.js:
- `main.wasp` — Declarative app definition (routes, auth, jobs, entities)
- `src/client/` — React frontend with Tailwind + Shadcn UI
- `src/server/` — Node.js backend with Express-like actions/queries
- Prisma ORM for database
- Fully typed end-to-end

## Extractable Modules

| Module | Difficulty | Est. Time | Target |
|--------|-----------|-----------|--------|
| Landing page design patterns | Needs adaptation | 3h | code-base/ui/landing-page/ |
| Stripe integration patterns | Needs rewrite (Wasp-specific) | 4h | Reference only |
| Auth flow architecture | Reference only (Wasp DSL) | — | Patterns reference |
| Background job patterns | Reference only | — | Patterns reference |

## 天子点评

功能最全的免费SaaS模板，没有之一——Auth/Stripe/邮件/后台任务/Landing Page全都有。但Wasp框架锁定是致命伤：你的代码和Wasp绑死，无法抽取模块到非Wasp项目。建议只作为"功能清单参考"和"Landing Page设计参考"，不建议直接基于它构建产品。选ixartz或自己从头搭。

## Risks / Why It Might Not Be Worth It

- **Wasp lock-in**: Framework-specific code can't be directly extracted
- **Not Next.js**: Uses React+Node, not Next.js — doesn't match base tech stack
- **114 open issues**: Some maintenance debt
- **Wasp learning curve**: Need to learn Wasp DSL before being productive
