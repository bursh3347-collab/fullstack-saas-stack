# Bulletproof React

> A simple, scalable, and powerful architecture guide for building production-ready React applications.

| Metric | Data |
|------|------|
| GitHub | [alan2207/bulletproof-react](https://github.com/alan2207/bulletproof-react) |
| Stars | 34,848 |
| Forks | 3,166 |
| License | MIT |
| Language | TypeScript |
| Last Updated | 2026-04-15 |
| Open Issues | 53 |
| Contributors | 60+ |

## TEMC Scores

| Dimension | Score | Reasoning |
|------|------|------|
| T (Tech) | 92 | Not a boilerplate — it's a comprehensive architecture guide. Covers project structure, components, state management, API layer, testing, performance, security. The React architecture bible. |
| E (Ecosystem) | 88 | 34.8k stars = one of the most starred React architecture resources. Referenced by countless tutorials, courses, and teams. alan2207 is a respected React educator. |
| M (Market) | 70 | Architecture guide, not a product template. Immense educational value but doesn't directly ship a SaaS. |
| C (Combo) | 85 | Architecture patterns directly applicable to any React/Next.js project. Feature-based folder structure is the gold standard. |
| **Overall** | **82.4** | T×0.25 + E×0.20 + M×0.30 + C×0.25 |

## Core Value

The definitive React application architecture guide:
- **Project Structure**: Feature-based organization
- **Components**: Atomic design + compound components
- **State Management**: When to use what (local vs global vs server)
- **API Layer**: React Query + typed API clients
- **Auth**: Authentication/authorization patterns
- **Testing**: Unit, integration, E2E strategy
- **Performance**: Code splitting, lazy loading, memoization
- **Error Handling**: Error boundaries, global error handling
- **Security**: XSS prevention, CSRF, input validation

## Architecture Highlights

Feature-based folder structure (the most influential pattern):
```
src/
├── features/           # Feature-based modules
│   ├── auth/
│   │   ├── api/        # API calls
│   │   ├── components/ # Feature-specific components
│   │   ├── hooks/      # Feature-specific hooks
│   │   ├── stores/     # Feature state
│   │   ├── types/      # TypeScript types
│   │   └── utils/      # Feature utilities
│   ├── users/
│   └── discussions/
├── components/         # Shared UI components
├── hooks/              # Shared hooks
├── lib/                # Configured library instances
├── stores/             # Global state
├── testing/            # Test utilities
├── types/              # Shared types
└── utils/              # Shared utilities
```

## Extractable Modules

| Module | Difficulty | Est. Time | Target |
|--------|-----------|-----------|--------|
| Feature-based folder structure | Simple copy | 0.5h | best-practices/architecture.md |
| React Query API patterns | Simple copy | 1h | code-base/api/react-query/ |
| Error boundary patterns | Simple copy | 1h | code-base/error-handling/ |
| Testing strategy | Reference | — | best-practices/testing.md |
| Auth patterns | Needs adaptation | 2h | code-base/auth/ |

⭐ **Universal Code Candidates**: Feature-based folder structure, Error boundaries, API layer patterns

## Risks / Why It Might Not Be Worth It

- Architecture guide, not runnable code — requires implementation effort
- Some patterns may be opinionated and not suit every project
- React-specific — doesn't cover full-stack concerns (DB, payments, etc.)
- 53 open issues suggest some community requests are unaddressed
