# Full-Stack SaaS Architecture Patterns

> Extracted from analysis of 5 top full-stack SaaS boilerplates. These patterns appear across multiple successful projects.

## 1. Feature-Based Folder Structure (from Bulletproof React)

The most widely adopted pattern across all analyzed projects:

```
src/
├── features/              # Domain-specific modules
│   ├── auth/              # Authentication feature
│   │   ├── api/           # API calls for auth
│   │   ├── components/    # Auth-specific UI
│   │   ├── hooks/         # Auth hooks (useAuth, useUser)
│   │   ├── stores/        # Auth state
│   │   ├── types/         # Auth TypeScript types
│   │   └── utils/         # Auth helpers
│   ├── billing/           # Payments/subscriptions
│   ├── teams/             # Team management
│   └── dashboard/         # Dashboard views
├── components/            # Shared UI components
├── hooks/                 # Shared hooks
├── lib/                   # Configured library instances
├── types/                 # Shared types
└── utils/                 # Shared utilities
```

**Why it works**: Each feature is self-contained. You can add/remove features without affecting others. New developers can find code by feature name.

## 2. API Layer Pattern (from FastAPI + Bulletproof React)

**Backend → OpenAPI → Generated Client → Frontend**

1. Backend defines API with type-safe models (SQLModel/Zod)
2. OpenAPI schema auto-generated
3. TypeScript client auto-generated from schema
4. Frontend uses generated client with React Query

**Benefit**: Zero type drift between frontend and backend. API changes caught at compile time.

## 3. Multi-Tenancy Architecture (from ixartz + BoxyHQ)

**Row-Level Security with Organization Scoping**:
```
User → belongs to → Organization (team)
Data → scoped by → Organization ID
Permissions → defined per → Role × Organization
```

Every database query includes org context. This enables:
- Data isolation between tenants
- Per-org billing
- Team collaboration features
- Enterprise SSO per organization

## 4. Auth Architecture Decision Tree

```
Need SSO/SAML?                    → BoxyHQ Jackson
Need social login + email/pass?   → NextAuth.js or Auth.js
API-first backend?                → JWT with refresh tokens (FastAPI pattern)
Full-stack Next.js?               → Auth.js + middleware
Need passwordless?                → Magic links (Supabase Auth)
```

## 5. Production Deployment Patterns

| Pattern | Used By | Best For |
|---------|---------|----------|
| Docker Compose + Traefik | FastAPI Full-Stack | Self-hosted, API-heavy |
| Vercel + Edge | ixartz, BoxyHQ | Next.js apps, fast iteration |
| Wasp deploy | Open SaaS | Wasp framework apps |
| Serverless functions | Various | Cost-efficient at low traffic |

## 6. Database Migration Pattern (Universal)

1. Schema-as-code (Prisma schema / SQLModel / Drizzle)
2. Auto-generate migrations from schema changes
3. Version control all migrations
4. Run migrations in CI/CD before deploy
5. Never manually edit production database

## 7. Naming Conventions (Synthesized from All Projects)

| Type | Convention | Example |
|------|-----------|----------|
| Files | kebab-case | `auth-provider.tsx` |
| Components | PascalCase | `AuthProvider` |
| Hooks | camelCase with `use` prefix | `useAuth` |
| API routes | kebab-case | `/api/auth/sign-in` |
| Database tables | snake_case | `user_profiles` |
| Environment vars | SCREAMING_SNAKE | `DATABASE_URL` |
