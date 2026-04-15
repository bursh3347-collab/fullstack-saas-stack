[English](README.md) | [中文](README_CN.md)

![Stars](https://img.shields.io/github/stars/bursh3347-collab/fullstack-saas-stack?style=flat-square)
![License](https://img.shields.io/github/license/bursh3347-collab/fullstack-saas-stack?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/bursh3347-collab/fullstack-saas-stack?style=flat-square)

# 🏗️ fullstack-saas-stack

> ⭐ **Maturity: L1 Growing** — 5 projects analyzed with TEMC scores, 2 best-practice guides, horizontal comparison.

Extracted best practices and analysis from top full-stack SaaS boilerplate projects on GitHub. Part of the [Open Source Knowledge Restructuring Project](https://github.com/bursh3347-collab).

## 📈 Category Overview

Full-stack SaaS boilerplates provide the foundation for building Software-as-a-Service applications. This repository analyzes the top projects, extracts their best patterns, and provides horizontal comparisons.

**Base Tech Stack**: TypeScript + Next.js + Tailwind/Shadcn + Supabase + Stripe + Vercel

## 📊 Project Rankings

| Rank | Project | Stars | TEMC | Best For |
|------|---------|-------|------|----------|
| 1 | [ixartz/SaaS-Boilerplate](projects/saas-boilerplate-ixartz.md) | 7.0k | **84.9** | 🏆 Best stack match |
| 2 | [alan2207/bulletproof-react](projects/bulletproof-react.md) | 34.8k | **82.4** | Architecture guide |
| 3 | [fastapi/full-stack-fastapi-template](projects/full-stack-fastapi-template.md) | 42.7k | **80.3** | Python full-stack |
| 4 | [wasp-lang/open-saas](projects/open-saas.md) | 14.1k | **79.6** | Free all-in-one |
| 5 | [boxyhq/saas-starter-kit](projects/saas-starter-kit-boxyhq.md) | 4.8k | **78.4** | Enterprise SSO |

## 📈 Trending Chart (Last Updated: 2026-04-15)

| Rank | Project | Total Stars | Weekly Growth | Trend |
|------|---------|-------------|---------------|-------|
| 1 | [FastAPI Full-Stack](projects/full-stack-fastapi-template.md) | 42.7k | ~80 | → Stable |
| 2 | [Bulletproof React](projects/bulletproof-react.md) | 34.8k | ~60 | → |
| 3 | [Open SaaS](projects/open-saas.md) | 14.1k | ~100 | ↑ Growing |
| 4 | [ixartz SaaS](projects/saas-boilerplate-ixartz.md) | 7.0k | ~50 | ↑ |
| 5 | [BoxyHQ](projects/saas-starter-kit-boxyhq.md) | 4.8k | ~20 | → |

> 📊 Stars data verified via GitHub API on 2026-04-15. Weekly growth is estimated based on trajectory.

## 📂 Repository Structure

```
fullstack-saas-stack/
├── projects/                 # Individual project analyses (TEMC format)
│   ├── saas-boilerplate-ixartz.md
│   ├── bulletproof-react.md
│   ├── full-stack-fastapi-template.md
│   ├── open-saas.md
│   └── saas-starter-kit-boxyhq.md
├── best-practices/           # Cross-project pattern extraction
│   ├── architecture.md       # Full-stack SaaS architecture patterns
│   └── auth-patterns.md      # Authentication comparison
├── code/                     # Extracted code (future)
├── comparison.md             # Horizontal comparison table
├── roadmap.md                # Category trends and future directions
├── SOURCES.md                # All source projects
├── CONTRIBUTING.md           # How to contribute
├── README.md                 # English (this file)
└── README_CN.md              # 中文版本
```

## 🏆 Key Takeaways

1. **Best stack match for solo devs**: ixartz/SaaS-Boilerplate (Next.js+Shadcn+TS)
2. **Best architecture reference**: Bulletproof React (feature-based structure)
3. **Best free all-in-one**: Open SaaS (but Wasp lock-in)
4. **Best for Python devs**: FastAPI Full-Stack Template
5. **Best for enterprise sales**: BoxyHQ (SSO+Audit)

## 🏷️ Solo Dev Verdict

Each project analysis includes a **Solo Dev Verdict** — a one-line assessment of whether the project is worth adopting for a one-person company.

## 📋 Universal Code Candidates

Modules identified for extraction to [code-base](https://github.com/bursh3347-collab/code-base):
- Docker Compose patterns (from FastAPI)
- Multi-tenancy architecture (from ixartz)
- RBAC permission system (from ixartz + BoxyHQ)
- Feature-based folder structure (from Bulletproof React)
- Audit log system (from BoxyHQ)
- JWT auth flow (from FastAPI)

## 🔗 Related Repositories

| Category | Repository | Maturity |
|----------|------------|----------|
| 🤖 AI Agent | [ai-agent-stack](https://github.com/bursh3347-collab/ai-agent-stack) | L2 Growing |
| 🏗️ Full-Stack SaaS | **fullstack-saas-stack** (this) | **L1 Growing** |
| 🎨 Frontend | [frontend-stack](https://github.com/bursh3347-collab/frontend-stack) | L1 Growing |
| 🔧 Code Base | [code-base](https://github.com/bursh3347-collab/code-base) | L1 Scaffolded |

## 📄 License

Analysis content: MIT. Individual projects retain their original licenses (see SOURCES.md).

---

*Powered by the TianGong Intelligence System — AI-driven open source intelligence engine*
