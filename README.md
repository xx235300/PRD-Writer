# PRD-Writer

English ｜ [[简体中文](https://github.com/xx235300/PRD-Writer/blob/main/README_zh.md)]

> **An AI-powered Product Requirements Document writing assistant — from raw ideas to structured, ready-to-build PRDs in minutes.**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Anthropic](https://img.shields.io/badge/Powered%20by-Anthropic-purple?style=flat-square&logo=anthropic)](https://www.anthropic.com)

Writing a good PRD is one of the most important — and most tedious — tasks in product development. PRD-Writer automates the tedious parts: the structure, the prioritization, and the acceptance criteria. You bring the product thinking; PRD-Writer brings the scaffolding.

Whether you have a rough idea, an existing draft that needs polishing, or a Feishu document you want to turn into a full PRD — PRD-Writer adapts to your workflow and delivers consistent, professional results in **English** or **Simplified Chinese**.

---

## Disclaimer

**Disclaimer**:
This project is 99% AI-generated. The AI's owner has no programming background. Please evaluate the project's feasibility before use.

---

## ✨ Key Advantages

| | |
|---|---|
| 🔄 **Anthropic 3-Phase Workflow** | Context Gathering → Refinement & Structure → Reader Testing |
| 📊 **MoSCoW Prioritization** | P0 / P1 / P2 / Won't — every feature has a clear priority label |
| ✅ **Given/When/Then Criteria** | BDD-style acceptance criteria your engineering team can execute directly |
| 🌐 **Bilingual Templates** | Full English and Simplified Chinese support with consistent structure |
| 🔗 **Feishu Doc Integration** | Read existing Feishu documents and generate or refine PRDs from them |
| 📐 **7-Chapter PRD Structure** | Complete, production-ready output covering every PRD essential |

---

## 🎯 Features

### 1. Three-Phase Scientific Workflow

PRD-Writer adopts Anthropic's proven collaborative writing methodology, ensuring AI and user form a clear, efficient collaboration loop:

- **Phase 1 — Context Gathering**: Active questioning to clarify product background, target users, core scenarios, and constraints
- **Phase 2 — Refinement & Structure**: Organizes all information into a complete 7-chapter PRD with MoSCoW-prioritized features
- **Phase 3 — Reader Testing**: Validates the document from a reader's perspective, confirms key decisions, and iterates on feedback

### 2. MoSCoW Prioritization Framework

No more vague "high/medium/low" labels. PRD-Writer applies the industry-standard MoSCoW framework to every feature:

| Priority | Label | Meaning |
|----------|-------|---------|
| **P0** | Must Have | Core functionality; a launch blocker if missing |
| **P1** | Should Have | High-impact features that significantly improve the product |
| **P2** | Could Have | Nice-to-have enhancements for the current release |
| **Won't** | Won't This Iteration | Explicitly deprioritized; future candidates |

### 3. Given/When/Then Acceptance Criteria

Every P0 and P1 feature includes acceptance criteria in the BDD-inspired Given/When/Then format:

```
Given  [precondition — system state before the action]
When   [trigger — the user's specific action]
Then   [expected outcome — observable, verifiable result]
```

Your engineering team can translate these directly into automated test cases. No more ambiguous acceptance criteria.

### 4. Bilingual Template Support

PRD-Writer ships with full English and Simplified Chinese PRD templates. Input your requirements in any language; output a structurally identical, professionally written PRD in your target language. Ideal for:

- **Cross-border product teams** collaborating across language barriers
- **Startups** building for both domestic and international markets
- **Freelancers** serving clients globally

### 5. Three Flexible Input Modes

Whether you're at the very beginning of a product idea or working from existing materials, PRD-Writer meets you where you are:

- **Mode A** — Raw idea → Complete PRD from scratch
- **Mode B** — Existing draft → Polished, restructured PRD
- **Mode C** — Feishu doc link → Iterative, multi-round PRD refinement

### 6. Complete 7-Chapter PRD Structure

Every output follows a proven, production-ready structure:

1. **Product Overview** — Vision, goals, scope, and value proposition
2. **User Analysis** — Personas and user journeys
3. **Feature Specifications** — MoSCoW-prioritized feature list and detailed descriptions
4. **Success Metrics** — North Star metric, leading and lagging indicators
5. **Acceptance Criteria** — Given/When/Then criteria for all P0/P1 features
6. **Technical Constraints** — Tech stack, integrations, security, and compliance
7. **Appendix** — Glossary, version history, and contacts

### 7. Feishu Cloud Document Integration

When you provide a Feishu document link (Feishu/Lark), PRD-Writer automatically reads its content, identifies gaps, and generates or refines a full PRD through multi-round collaboration.

---

## 📦 Installation

### Option 1: Clone from GitHub

```bash
git clone https://github.com/your-org/prd-writer.git
cd prd-writer
# Follow the setup instructions in the repository
```

### Option 2: Install via ClawHub

```bash
# Use the ClawHub CLI to install PRD-Writer as an OpenClaw skill
clawhub install prd-writer
```

> **Prerequisites**: Node.js 18+, npm 9+, and an active OpenClaw installation.
> For detailed installation instructions, see the [User Guide 📖](#-faq).

---

## 🚀 Quick Start

### Step 1 — Activate the Skill

In any conversation, trigger PRD-Writer using any of the [11 trigger words](#-trigger-words), for example:

```
write a PRD
```
or in Chinese:
```
写PRD
```

### Step 2 — Answer a Few Clarifying Questions

PRD-Writer enters **Phase 1 (Context Gathering)** and asks 2–3 targeted questions about your product idea:

- Who is the target user?
- What are the top 3 core features?
- What does success look like (quantifiable)?

> Answer as many or as few as you can. PRD-Writer will use `[待确认]` placeholders for anything unspecified.

### Step 3 — Receive Your Complete PRD

PRD-Writer enters **Phase 2** and generates the full 7-chapter PRD with:

- ✅ MoSCoW-prioritized feature list
- ✅ Given/When/Then acceptance criteria for every P0/P1 feature
- ✅ Completion indicators on each chapter (✅ = complete, ⚠️ = needs confirmation)

Then **Phase 3** asks you to review and confirm key decisions before finalizing.

---

## 🔄 Three-Phase Workflow

### Phase 1 — Context Gathering

**Goal**: Collect enough background to write the PRD without guessing.

PRD-Writer collects information across 8 dimensions, one at a time:

| Dimension | PRD Chapter | Example Question |
|-----------|------------|-----------------|
| Project background & goals | Product Overview | What problem does this product solve? |
| Target users | User Analysis | Who are the primary users and what are their pain points? |
| Core features | Feature Specifications | What are the top 3 must-have features? |
| Priority decisions | Feature Specifications | What gets cut if you only have 2 weeks? |
| Success metrics | Success Metrics | What quantifiable outcome do you expect? |
| Acceptance criteria | Acceptance Criteria | What does "done" look like for the core feature? |
| Technical constraints | Technical Constraints | Any platform, tech stack, or integration limits? |
| Output format | Delivery | Should I write this to a Feishu doc or reply here? |

PRD-Writer asks 2–3 questions per round to avoid overwhelming you. At the end of Phase 1, it outputs a **Context Checklist** for your confirmation before generating the document.

---

### Phase 2 — Refinement & Structure

**Goal**: Generate a complete, well-structured PRD document.

Based on confirmed context, PRD-Writer produces all 7 chapters in order of priority:

| Order | Chapter | Priority |
|-------|---------|----------|
| 1 | Product Overview | P0 (mandatory) |
| 2 | User Analysis | P0 (mandatory) |
| 3 | Feature Specifications (MoSCoW) | P0 (mandatory) |
| 4 | Success Metrics | P1 (should have) |
| 5 | Acceptance Criteria (Given/When/Then) | P1 (should have) |
| 6 | Technical Constraints | P2 (could have) |
| 7 | Appendix | P2 (could have) |

> Any information not provided by the user is marked with `[待确认]` and flagged in the chapter's completion indicator.

---

### Phase 3 — Reader Testing

**Goal**: Validate clarity, completeness, and consistency before final delivery.

PRD-Writer reviews the completed PRD from the reader's perspective, covering:

- ✅ Does the Product Overview clearly explain *why* we are building this?
- ✅ Are target users and their journeys complete?
- ✅ Are P0/P1/P2 priorities aligned with your business goals?
- ✅ Are Given/When/Then criteria specific and verifiable?
- ✅ Are success metric target values realistic?

PRD-Writer also surfaces **key decision points** for explicit confirmation:

> "The target for first response time is 24 hours. Would you prefer a more aggressive target like 4 hours, or a more conservative one like 48 hours?"

You can request updates to any chapter at any time. PRD-Writer marks changes with a version diff (e.g., `[v0.9 → v0.91]`).

---

## 💬 Trigger Words

PRD-Writer activates when you use **any** of the following trigger words or phrases. Use them in either English or Chinese — PRD-Writer auto-detects the language and adapts.

| # | English Trigger | 中文触发词 |
|---|----------------|-----------|
| 1 | `write a PRD` | 写PRD |
| 2 | `create a PRD` | 做PRD |
| 3 | `generate PRD` | 生成PRD |
| 4 | `PRD writing` | PRD写作 |
| 5 | `requirements document` | 需求文档 |
| 6 | `product requirements document` | 产品需求文档 |
| 7 | `write a requirements document` | 编写需求文档 |
| 8 | `prd-writer` | prd-writer |
| 9 | `product document` | 产品文档 |
| 10 | `output a PRD` | 输出PRD |
| 11 | `PRD template` | PRD模板 |

> **Tip**: You don't need an exact match — PRD-Writer understands intent. Just say "I need a PRD for a new feature" and it activates automatically.

---

## 📥 Input Modes

### Mode A — Plain Idea → Complete PRD

**Best for**: Products from 0 to 1, or new features with no existing documentation.

You describe your product idea in plain language — rough, incomplete, and conversational is fine:

```
You: I want to build a user feedback system where customers can submit
     issues and get notified when they're resolved.
```

PRD-Writer activates → asks 2–3 clarifying questions → generates the full 7-chapter PRD.

---

### Mode B — Existing Draft → Polished PRD

**Best for**: Unstructured notes, half-written drafts, or outdated PRDs that need a refresh.

You paste your existing content:

```
You: [paste a rough PRD draft or bullet-point wishlist]
```

PRD-Writer analyzes it → identifies missing chapters and content gaps → asks targeted follow-up questions → outputs a fully structured, prioritized PRD.

---

### Mode C — Feishu Doc Link → Multi-round PRD

**Best for**: Teams already working in Feishu who have scattered requirements across multiple documents.

You share a Feishu document URL:

```
You: https://feishu.cn/doc/xxxxx — Generate a PRD from this.
```

PRD-Writer reads the document → identifies gaps → confirms missing info with you → generates a polished PRD. Supports multi-round iteration for partial updates to specific chapters.

---

## ❓ FAQ

### Q: How is PRD-Writer different from just asking an AI to write a PRD?

Most AIs generate a generic, template-filling document. PRD-Writer follows a **structured three-phase workflow** — it asks targeted questions, applies **MoSCoW prioritization**, and outputs **Given/When/Then acceptance criteria** that your engineering team can act on directly. The output is not just text; it's a working document with verifiable completion criteria.

### Q: Does PRD-Writer support languages other than English and Chinese?

Currently, the full template and workflow are optimized for **English** and **Simplified Chinese**. Other languages are partially supported — the workflow functions, but template labels and section headers will fall back to English.

### Q: Where can I find the full user guide?

The complete user guide with detailed examples, troubleshooting, and advanced usage tips is available in the [飞书云文档用户指南 📖](https://your-feishu-doc-link).

### Q: Can I request changes to a specific chapter after the PRD is generated?

Yes. PRD-Writer supports **partial updates**. Simply tell it which chapter to revise (e.g., "Please update Chapter 3 — add a P1 feature for email notifications"). Changes are marked with a version diff.

### Q: How are `[待确认]` placeholders handled?

Items marked `[待确认]` indicate information you did not provide during Context Gathering. PRD-Writer will not guess — it leaves a clear placeholder so you know exactly what needs a business decision. You can fill these in later by telling PRD-Writer to update the specific section.

### Q: Can I output the PRD directly to Feishu?

Yes. When you trigger PRD-Writer, specify your preferred output method:
- **Default**: Markdown output in the conversation
- **Optional**: Written directly to a Feishu Cloud Document (provide the folder or wiki link)

---

## 🙏 Credit & Acknowledgment

PRD-Writer's design philosophy draws direct inspiration from **Anthropic's official doc-coauthoring project**, which pioneered the application of large language model collaboration techniques to structured document creation.

The **three-phase workflow** — **Context Gathering → Refinement & Structure → Reader Testing** — is directly derived from Anthropic's collaborative writing methodology. Anthropic demonstrated how structured AI collaboration can transform open-ended document tasks into efficient, high-quality outputs.

We are grateful to the Anthropic team for advancing the state of the art in AI-assisted writing and documentation, and for providing a framework that PRD-Writer builds upon.

---

*Last updated: 2026-03-28 | PRD-Writer v1.0*
