[English](README.md) | [中文](README_CN.md)

# 🏗️ fullstack-saas-stack

> ⭐ **成熟度：L1 成长期** — 已分析5个项目（含TEMC评分），2份最佳实践指南，横向对比表。

从GitHub高星全栈SaaS模板项目中提取最佳实践与分析。属于[开源知识重组工程](https://github.com/bursh3347-collab)的一部分。

## 📈 分类概览

全栈SaaS模板为构建SaaS应用提供基础。本仓库分析顶级项目、提取最佳模式、提供横向对比。

**基准技术栈**：TypeScript + Next.js + Tailwind/Shadcn + Supabase + Stripe + Vercel

## 📊 项目排名

| 排名 | 项目 | Stars | TEMC | 最适合 |
|------|------|-------|------|--------|
| 1 | [ixartz/SaaS-Boilerplate](projects/saas-boilerplate-ixartz.md) | 7.0k | **84.9** | 🏆 技术栈最匹配 |
| 2 | [alan2207/bulletproof-react](projects/bulletproof-react.md) | 34.8k | **82.4** | 架构参考 |
| 3 | [fastapi/full-stack-fastapi-template](projects/full-stack-fastapi-template.md) | 42.7k | **80.3** | Python全栈 |
| 4 | [wasp-lang/open-saas](projects/open-saas.md) | 14.1k | **79.6** | 免费一站式 |
| 5 | [boxyhq/saas-starter-kit](projects/saas-starter-kit-boxyhq.md) | 4.8k | **78.4** | 企业级SSO |

## 📈 飙升榜（最近更新：2026-04-15）

| 排名 | 项目 | 总Stars | 周增 | 趋势 |
|------|------|---------|------|------|
| 1 | [FastAPI Full-Stack](projects/full-stack-fastapi-template.md) | 42.7k | ~80 | → 稳定 |
| 2 | [Bulletproof React](projects/bulletproof-react.md) | 34.8k | ~60 | → |
| 3 | [Open SaaS](projects/open-saas.md) | 14.1k | ~100 | ↑ 增长 |
| 4 | [ixartz SaaS](projects/saas-boilerplate-ixartz.md) | 7.0k | ~50 | ↑ |
| 5 | [BoxyHQ](projects/saas-starter-kit-boxyhq.md) | 4.8k | ~20 | → |

> 📊 Stars数据于2026-04-15通过GitHub API验证。周增为基于增长轨迹的估算值。

## 🏆 核心结论

1. **独立开发者最佳选择**：ixartz/SaaS-Boilerplate（Next.js+Shadcn+TS）
2. **最佳架构参考**：Bulletproof React（基于功能的目录结构）
3. **最佳免费一站式**：Open SaaS（但有Wasp锁定风险）
4. **Python开发者首选**：FastAPI Full-Stack Template
5. **企业销售最佳**：BoxyHQ（SSO+审计日志）

## 🏷️ 独立开发者点评

每个项目分析都包含 **独立开发者点评** —— 一句话评估该项目是否值得一人公司采用。

## 📋 通用代码候选

已识别可提取到 [code-base](https://github.com/bursh3347-collab/code-base) 的模块：
- Docker Compose模式（来自FastAPI）
- 多租户架构（来自ixartz）
- RBAC权限系统（来自ixartz + BoxyHQ）
- 基于功能的目录结构（来自Bulletproof React）
- 审计日志系统（来自BoxyHQ）
- JWT认证流程（来自FastAPI）

## 🔗 相关仓库

| 分类 | 仓库 | 成熟度 |
|------|------|--------|
| 🤖 AI Agent | [ai-agent-stack](https://github.com/bursh3347-collab/ai-agent-stack) | L2 成长期 |
| 🏗️ 全栈SaaS | **fullstack-saas-stack**（本仓库） | **L1 成长期** |
| 🎨 前端 | [frontend-stack](https://github.com/bursh3347-collab/frontend-stack) | L1 成长期 |
| 🔧 通用代码库 | [code-base](https://github.com/bursh3347-collab/code-base) | L1 脚手架 |

## 📄 许可证

分析内容：MIT。各项目保留其原始许可证（详见 SOURCES.md）。

---

*由天工情报系统驱动 — AI驱动的开源知识引擎*
