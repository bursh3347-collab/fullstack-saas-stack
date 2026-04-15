# Authentication Patterns in SaaS Applications

> Comparative analysis of auth implementations across 5 top SaaS boilerplates.

## Auth Implementation Comparison

| Project | Auth Method | Providers | Session Type | Multi-tenant |
|---------|-----------|-----------|-------------|-------------|
| FastAPI | JWT (custom) | Email/pass | Bearer token | No |
| Open SaaS | Wasp Auth | Email/Google/GitHub/Slack/MS | Session-based | No |
| ixartz | NextAuth/Auth.js | Multiple | JWT + Session | Yes (per-org) |
| BoxyHQ | NextAuth + Jackson | SSO/SAML/OIDC | Session-based | Yes (per-org) |
| Bulletproof | Patterns only | — | — | — |

## Pattern 1: JWT with Refresh Tokens (FastAPI)

Best for: API-first backends, mobile apps

```
Login → Access Token (15min) + Refresh Token (7d)
API Call → Authorization: Bearer <access_token>
Expired → Use refresh token to get new access token
Logout → Revoke refresh token
```

**Pros**: Stateless, works across services, good for mobile
**Cons**: Token revocation requires blocklist, larger request headers

## Pattern 2: Session-Based with Auth.js (ixartz/BoxyHQ)

Best for: Full-stack Next.js, server-rendered pages

```
Login → Server creates session → Cookie set
Page Load → Middleware checks session → Redirect if invalid
API Call → Session ID from cookie → Server validates
Logout → Delete session
```

**Pros**: Simple, secure by default, easy revocation
**Cons**: Requires server-side session storage, sticky sessions in multi-server

## Pattern 3: Enterprise SSO (BoxyHQ Jackson)

Best for: B2B SaaS selling to enterprises

```
Org Admin → Configures SAML/OIDC connection
Employee → Clicks "Login with SSO" → Redirected to IdP
IdP → Authenticates → Redirects back with assertion
App → Validates assertion → Creates/updates user session
```

**When to add SSO**: When your first enterprise customer asks for it (it's the #1 enterprise upsell).

## Recommended Auth Stack for One-Person Company

**Start with**: Auth.js (NextAuth) — free, battle-tested, multiple providers
**Add later**: BoxyHQ Jackson — when enterprise customers need SSO
**Consider**: Supabase Auth — if already using Supabase for database
