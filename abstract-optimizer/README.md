# abstract-optimizer — 摘要优化与审查 / Abstract Review & Optimization Toolkit

[![version](https://img.shields.io/badge/version-1.0.0-blue)]()

**中文** | [English](#english)

---

## 中文

### 这是什么？

`abstract-optimizer` 是一个**摘要质量审查与优化工具箱**，专门服务于中文学术论文的中英文摘要。它不是摘要生成器，而是在摘要写完之后，帮你：

- 🔍 审查中英文摘要是否**内容对称**（数据、关键词、要素一一对应）
- 📐 检查摘要是否符合**学科规范模板**（工程/管理/医学/CS）
- 🔗 验证摘要中的每个数据声明，是否都能在**正文中找到对应**
- ✅ 用 **30项标准化清单**逐条打分，发现隐形问题
- 🏷️ 优化关键词选取，让论文更易被检索发现

### 为什么需要它？

SkillHub 上已有的摘要工具（`abstract-summarizer`、`abstract-trimmer`、`abstract-logic-writer`、`conference-abstract-adaptor`）全部围绕**生成、裁剪、评分、格式适配**——它们帮你"写"摘要。但写完之后的**质量审查、中英对称、正文一致性验证**，无人覆盖。本技能填补这个空缺。

### 适用场景

- 投稿前检查
- 学位论文摘要审查
- 中英双语摘要同步修订
- 关键词优化以提升数据库检索命中率

### 快速上手

1. 向Agent提交你的中文摘要 + 英文摘要（可选：论文正文片段）
2. Agent将调用对应的审查子模块，输出审查报告
3. 根据优化建议修改摘要

### 文件说明

```
abstract-optimizer/
├── SKILL.md                         ← 技能主文件
├── README.md                        ← 本文件
└── references/
    ├── cn-en-abstract-spec.md       ← 核心规范
    ├── discipline-templates.md      ← 学科模板
    ├── abstract-body-mapping.md     ← 摘要-正文映射
    ├── abstract-review-checklist.md ← 30项审查清单
    └── keyword-optimization.md      ← 关键词优化
```

---

## English

### What Is This?

`abstract-optimizer` is an **academic abstract quality review and optimization toolkit** for bilingual (Chinese-English) academic papers. It is NOT a generator — it reviews, validates, and optimizes abstracts after they are drafted:

- 🔍 **CN-EN Symmetry Check**: Verify content correspondence, data consistency, keyword alignment, and tense matching between Chinese and English abstracts
- 📐 **Discipline Templates**: Match your abstract against field-specific templates (Engineering, Management, Medicine, CS)
- 🔗 **Body-Abstract Mapping**: Extract every factual claim from the abstract and verify it against the paper body
- ✅ **30-Item Checklist**: Systematic review across 6 categories
- 🏷️ **Keyword Optimization**: Ensure keywords are well-chosen, conceptually aligned in both languages, and optimized for database discovery

### Why Do You Need It?

Existing SkillHub abstract tools (`abstract-summarizer`, `abstract-trimmer`, `abstract-logic-writer`, `conference-abstract-adaptor`) all focus on *generating, trimming, scoring, or formatting* abstracts. They help you *write* the abstract. What's missing is *post-writing quality review* — symmetry checks, consistency verification, and optimization. This skill fills that gap.

### Use Cases

- Pre-submission quality check
- Thesis/dissertation abstract review
- Bilingual abstract synchronization
- Keyword optimization for better search retrieval

### Quick Start

1. Submit your Chinese abstract + English abstract (optionally: body text excerpts)
2. The Agent will invoke the relevant review sub-modules and generate a review report
3. Revise the abstract based on optimization suggestions

### File Structure

See the Chinese section above for the file tree.

---

## 触发词一览 / Trigger Keywords

| 中文 | English |
|------|---------|
| 摘要优化 | abstract optimization |
| 摘要审查 | abstract review |
| 中英摘要 | CN-EN abstract |
| 摘要对称 | abstract symmetry |
| 摘要规范 | abstract specification |
| 摘要与正文映射 | abstract-body mapping |
| 关键词优化 | keyword optimization |
| 摘要质量审查 | abstract quality check |
| 摘要合规检查 | abstract compliance check |

---

*All examples in the reference files use fictitious paper titles and abstract content. No real papers, authors, or data are referenced.*

---

作者：刘楠
