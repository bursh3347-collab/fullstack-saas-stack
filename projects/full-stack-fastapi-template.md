# Full Stack FastAPI Template

> The official FastAPI full-stack template with React, SQLModel, PostgreSQL, Docker, and automatic HTTPS.

| Metric | Data |
|------|------|
| GitHub | [fastapi/full-stack-fastapi-template](https://github.com/fastapi/full-stack-fastapi-template) |
| Stars | 42,647 |
| Forks | 8,384 |
| License | MIT |
| Language | TypeScript + Python |
| Last Updated | 2026-04-15 |
| Open Issues | 24 |
| Contributors | 100+ |

## TEMC Scores

| Dimension | Score | Reasoning |
|------|------|------|
| T (Tech) | 88 | Production-grade architecture: FastAPI+SQLModel backend, React+TypeScript frontend, Docker Compose, Traefik reverse proxy, automatic HTTPS, GitHub Actions CI/CD. Excellent code quality and documentation. |
| E (Ecosystem) | 90 | 42.6k stars, official FastAPI project by Sebastián Ramírez (tiangolo). Massive community, 8.3k forks. Active maintenance by FastAPI core team. |
| M (Market) | 75 | Python-first full-stack template. Strong for Python developers but TypeScript-first SaaS market prefers Next.js. Great for API-heavy products. |
| C (Combo) | 72 | Python backend diverges from base tech stack (TS+Next.js). However, FastAPI patterns are excellent reference for API design. Docker setup is reusable. |
| **Overall** | **80.3** | T×0.25 + E×0.20 + M×0.30 + C×0.25 |

## Core Value

The gold standard for Python full-stack development. Provides a battle-tested production architecture with:
- **FastAPI** backend with auto-generated OpenAPI docs
- **SQLModel** for type-safe database operations
- **React + TypeScript** frontend with Chakra UI
- **Docker Compose** for local dev and production
- **Traefik** for automatic HTTPS and load balancing
- **GitHub Actions** CI/CD pipeline
- **JWT authentication** with secure defaults

## Architecture Highlights

```
full-stack-fastapi-template/
├── backend/           # FastAPI + SQLModel + Alembic migrations
│   ├── app/
│   │   ├── api/       # API routes (users, items, login, utils)
│   │   ├── core/      # Config, security, DB engine
│   │   ├── models/    # SQLModel models
│   │   └── tests/     # Pytest test suite
│   └── alembic/       # Database migrations
├── frontend/          # React + TypeScript + Vite
│   ├── src/
│   │   ├── client/    # Auto-generated API client from OpenAPI
│   │   ├── components/# React components
│   │   ├── hooks/     # Custom hooks
│   │   └── routes/    # TanStack Router pages
│   └── tests/         # Playwright E2E tests
├── docker-compose.yml # Full stack orchestration
└── .github/workflows/ # CI/CD
```

**Key Pattern**: Auto-generated TypeScript API client from FastAPI's OpenAPI schema — eliminates frontend/backend type drift.

## Extractable Modules

| Module | Difficulty | Est. Time | Target |
|--------|-----------|-----------|--------|
| Docker Compose multi-service setup | Simple copy | 1h | code-base/deploy/docker/ |
| JWT auth flow (backend) | Needs adaptation | 3h | code-base/auth/jwt/ |
| OpenAPI → TypeScript client generation | Simple copy | 1h | code-base/api/openapi-codegen/ |
| Alembic migration patterns | Simple copy | 1h | code-base/database/migrations/ |
| GitHub Actions CI/CD | Needs adaptation | 2h | code-base/deploy/ci-cd/ |

⭐ **Universal Code Candidates**: Docker Compose patterns, CI/CD workflows, JWT auth flow

## Business Value

- **Pain Point**: Setting up a production Python full-stack app from scratch (Level: Important)
- **Target Users**: Python developers building APIs, data-heavy applications, ML-powered products
- **TAM**: Large — Python web dev market
- **Differentiation Window**: The only official FastAPI template; competitors (cookiecutter-django, etc.) are less modern

## Risks / Why It Might Not Be Worth It

- Python backend doesn't match base tech stack (TypeScript+Next.js)
- React frontend uses Chakra UI (not shadcn/Tailwind)
- Heavier Docker-first setup vs serverless (Vercel) approach
- Overkill for simple CRUD apps
