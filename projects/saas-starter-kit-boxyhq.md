# SaaS Starter Kit by BoxyHQ

> Enterprise SaaS Starter Kit with Next.js — SSO, Directory Sync, Audit Logs, and more.

| Metric | Data |
|------|------|
| GitHub | [boxyhq/saas-starter-kit](https://github.com/boxyhq/saas-starter-kit) |
| Stars | 4,772 |
| Forks | 1,199 |
| License | Apache-2.0 |
| Language | TypeScript |
| Last Updated | 2026-04-14 |
| Open Issues | 39 |
| Contributors | 40+ |

## TEMC Scores

| Dimension | Score | Reasoning |
|------|------|------|
| T (Tech) | 85 | Next.js + Tailwind + TypeScript. Enterprise features: SSO (SAML/OIDC), Directory Sync (SCIM), Audit Logs, Webhooks. Backed by BoxyHQ (enterprise identity company). |
| E (Ecosystem) | 68 | 4.8k stars. Backed by BoxyHQ company. Smaller community but enterprise-focused. 1.2k forks shows real adoption. |
| M (Market) | 78 | Enterprise SaaS features that startups need to sell to enterprise customers. SSO and audit logs are the #1 enterprise upsell features. |
| C (Combo) | 80 | Next.js + Tailwind + TypeScript matches base stack. Enterprise features (SSO, audit logs) are premium upsell modules for any SaaS. |
| **Overall** | **78.4** | T×0.25 + E×0.20 + M×0.30 + C×0.25 |

## Core Value

Enterprise-grade SaaS features out of the box:
- **SSO**: SAML + OIDC single sign-on via BoxyHQ
- **Directory Sync**: SCIM provisioning
- **Audit Logs**: Enterprise compliance logging
- **Webhooks**: Event-driven integrations
- **Team Management**: Invite, roles, permissions
- **Next-Auth**: Authentication backbone
- **Prisma**: Database ORM
- **Tailwind CSS**: Styling

## Architecture Highlights

```
saas-starter-kit/
├── components/       # React components
├── lib/              # Core libraries
│   ├── jackson/      # BoxyHQ SSO integration
│   ├── prisma/       # Database client
│   └── permissions/  # RBAC system
├── models/           # Data models
├── pages/            # Next.js pages
│   ├── api/          # API routes
│   ├── auth/         # Auth pages
│   └── teams/        # Team management
└── prisma/           # Schema + migrations
```

**Key Pattern**: Enterprise feature modules (SSO, SCIM, Audit) are cleanly separated and can be toggled on/off.

## Extractable Modules

| Module | Difficulty | Est. Time | Target |
|--------|-----------|-----------|--------|
| Audit log system | Needs adaptation | 3h | code-base/monitoring/audit-logs/ |
| Webhook system | Needs adaptation | 2h | code-base/api/webhooks/ |
| Team invitation flow | Simple copy | 2h | code-base/auth/team-invites/ |
| RBAC permissions | Needs adaptation | 2h | code-base/auth/rbac/ |

⭐ **Universal Code Candidates**: Audit log pattern, Webhook system, Team management

## 天子点评

企业级SaaS的必备参考——SSO/SCIM/Audit Log这三样是向企业客户收费的核心功能。但对早期Micro SaaS来说太重了，4.8k Stars也说明不是大众选择。建议策略：先用ixartz快速上线，等有企业客户需求时再来这里抄SSO和Audit Log模块。注意它用的是Pages Router（旧架构），需要迁移到App Router。

## Risks / Why It Might Not Be Worth It

- BoxyHQ dependency for SSO — adds vendor lock-in for enterprise features
- Smaller community (4.8k stars)
- Next.js Pages Router (not App Router) — older architecture
- Enterprise features may be overkill for early-stage Micro SaaS
- BoxyHQ company backing is double-edged: stable funding but commercial interests
