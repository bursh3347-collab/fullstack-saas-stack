# 🗺️ Full-Stack SaaS Stack — Technology Roadmap

> 当前主流 / 崛起方向 / 衰退方向 / 6-12月预测 / 对一人公司的影响

*Last Updated: 2026-04-15*

## 🟢 当前主流方向

### 1. Next.js App Router + Server Components
- **代表项目**: ixartz/SaaS-Boilerplate (7.0k⭐)
- **趋势**: App Router成为Next.js SaaS的默认架构，Server Components减少客户端JS
- **成熟度**: 中期（自我强化）
- **一人公司影响**: ⭐ **基准选择** — App Router + RSC是2026年SaaS标配

### 2. Shadcn UI + Tailwind CSS
- **趋势**: 取代Material UI/Chakra UI成为React UI首选
- **成熟度**: 中期→晚期（共识已形成）
- **一人公司影响**: 零争议的UI选择，所有新SaaS模板都在用

### 3. Type-Safe Full-Stack (Drizzle/Prisma + tRPC/Server Actions)
- **趋势**: 端到端类型安全从Nice-to-have变为Must-have
- **成熟度**: 中期
- **一人公司影响**: Drizzle比Prisma更轻量，推荐作为默认ORM

## 🚀 崛起方向

### 4. AI-Native SaaS Templates
- **信号**: Open SaaS增加AGENTS.md和Claude Code插件
- **趋势**: SaaS模板从"含AI功能"进化为"AI-first架构"（Agent内建）
- **成熟度**: 早期
- **一人公司影响**: 下一代SaaS模板将默认包含Agent/RAG/Memory模块

### 5. Serverless-First Deployment
- **趋势**: Vercel/Cloudflare Workers取代Docker Compose成为默认部署方式
- **成熟度**: 中期
- **一人公司影响**: 零运维部署 = 一人公司的最佳选择

### 6. Multi-Tenancy as Default
- **代表**: ixartz (organization-based), BoxyHQ (team-based)
- **趋势**: 多租户从企业功能变为SaaS标配
- **一人公司影响**: 提前内建multi-tenancy，避免后期重构

### 7. Payments Beyond Stripe
- **信号**: Open SaaS集成Polar.sh，Lemon Squeezy崛起
- **趋势**: 支付提供商多元化，Merchant of Record模式降低合规成本
- **一人公司影响**: Stripe仍是首选，但Polar.sh/Lemon Squeezy对个人开发者更友好

## ⬇️ 衰退方向

### 8. Pages Router Architecture
- **信号**: BoxyHQ仍用Pages Router（旧架构）
- **趋势**: Pages Router不再是新项目的推荐选择
- **一人公司影响**: 新项目必须用App Router

### 9. Framework Lock-in Templates
- **信号**: Wasp/Blitz等DSL框架增长放缓
- **趋势**: 开发者更偏好可脱离框架的标准架构
- **一人公司影响**: 避免框架锁定，选择标准Next.js方案

### 10. Paid SaaS Boilerplates ($200-500)
- **信号**: 免费替代品质量快速提升（ixartz, Open SaaS）
- **趋势**: 付费模板的价值空间被压缩
- **一人公司影响**: 免费方案已足够好，无需付费购买

## 🔮 6-12个月预测

1. **Next.js 16 + React 19 Server Components** 将成为所有SaaS模板的基线
2. **AI Agent集成** 将成为SaaS boilerplate的标准模块（不再是可选插件）
3. **Edge Runtime** 部署将取代传统Node.js runtime成为默认
4. **Auth.js v5 (NextAuth) + Passkey** 将替代传统密码登录
5. **Stripe Billing v2 + Usage-Based Pricing** 将成为AI SaaS的标准计费模式

## 💡 对一人公司的行动建议

| 优先级 | 行动 | 预估时间 | 依据 |
|--------|------|----------|------|
| P0 | Fork ixartz/SaaS-Boilerplate作为基座 | 1h | TEMC最高分，完美栈匹配 |
| P0 | 参考Bulletproof React搭建项目结构 | 1h | Feature-based架构金标准 |
| P1 | 集成Stripe订阅 + Landing Page | 4h | 变现核心 |
| P1 | 添加AI Agent模块（OpenAI SDK） | 4h | AI-Native差异化 |
| P2 | 学习BoxyHQ的SSO/Audit Log模式 | 2h | 企业客户升级路径 |
| P3 | 研究FastAPI的Docker部署模式 | 2h | 需要Python后端时参考 |

---

*This roadmap is maintained by [天工系统](https://github.com/bursh3347-collab) and updated with each scan cycle.*
