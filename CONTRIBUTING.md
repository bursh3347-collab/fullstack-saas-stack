# 🤝 Contributing to fullstack-saas-stack

Thank you for your interest! This repository is part of the **GitHub Open Source Knowledge Restructuring Project** — we deeply analyze SaaS boilerplate projects, extract patterns, and provide actionable comparisons.

## 📋 How to Contribute

### 1. Add a New Project Analysis

Create `projects/[project-name].md` following the **TEMC template**:

```markdown
# Project Name

> One-line description

| Metric | Data |
|--------|------|
| GitHub | [owner/repo](link) |
| Stars | X,XXX |
| Forks | X,XXX |
| License | MIT/Apache/... |
| Language | Language |
| Last Updated | YYYY-MM-DD |
| Open Issues | XX |
| Contributors | XX |

## TEMC Scores

| Dimension | Score | Reasoning |
|-----------|-------|-----------|
| T (Tech) | XX | Data-backed |
| E (Ecosystem) | XX | Data-backed |
| M (Market) | XX | Data-backed |
| C (Combo) | XX | Data-backed |
| **Overall** | **XX** | T×0.25 + E×0.20 + M×0.30 + C×0.25 |

## Core Value
## Architecture Highlights
## Extractable Modules
## 天子点评
## Risks / Why It Might Not Be Worth It
```

### 2. Submit Code Extractions

When extracting reusable code:
- Place in `code/[module-name]/` with a README
- Include source attribution and license
- Must be runnable — not just snippets
- Mark cross-category patterns with ⭐ for `code-base/` extraction

### 3. Update Supporting Files

After adding a project:
- [ ] Update `comparison.md` with the new project
- [ ] Update `SOURCES.md` with Stars, License, analysis date
- [ ] Update `README.md` rankings if score places in top 5

## ✅ Quality Standards

- Every TEMC score **must be backed by specific data**
- Every project **must include a 反证/Risks section**
- Every project **must include a 天子点评 section**
- Stars > 500 threshold (exceptions with justification)
- Active commits within last 90 days
- Permissive license: MIT / Apache-2.0 / BSD

## 📝 PR Template

```
## What this PR does
<!-- Brief description -->

## Checklist
- [ ] Project analysis follows TEMC template
- [ ] TEMC scores backed by specific data
- [ ] 反证/Risks section included
- [ ] 天子点评 section included
- [ ] SOURCES.md updated
- [ ] comparison.md updated (if applicable)
- [ ] License verified as permissive
```

## 🏷️ Good First Issues

- **Update Stars count**: Verify Stars match current GitHub data
- **Add missing 天子点评**: Some early projects may lack this section
- **Translate content**: Add English/Chinese translations
- **Fix typos/links**: PRs welcome!
- **Add a new SaaS boilerplate**: Know a Stars>500 project not yet analyzed?

---

*Powered by [天工系统](https://github.com/bursh3347-collab) — AI-driven open source intelligence engine*
