<div align="center">

# Research Before Build

### Find before inventing. Verify before deciding. Blueprint before building.

A reusable Agent Skill that teaches coding agents to research **skills, official docs, implementation patterns, competitors, market evidence, failures, and pricing** before they build an AI agent, website, SaaS, automation, or digital offer.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Skill](https://img.shields.io/badge/Agent%20Skill-SKILL.md-6f42c1)
![Research](https://img.shields.io/badge/workflow-research%20%E2%86%92%20decision%20%E2%86%92%20build-0969da)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

</div>

## Why this exists

AI coding agents are excellent at producing output quickly. That becomes a liability when they start coding before checking whether a strong skill already exists, whether the framework changed recently, whether official docs recommend a different primitive, whether a known production failure already has a pattern, or whether customers actually care about the proposed feature.

**Research Before Build** adds a reusable pre-build operating system:

```text
REQUEST
   ↓
CLASSIFY
   ↓
FIND EXISTING SKILLS
   ↓
RESEARCH CURRENT SOURCES
   ↓
TRIANGULATE + VERIFY
   ↓
DECIDE
   ↓
BLUEPRINT
   ↓
BUILD
   ↓
VALIDATE
```

The goal is not "more research". The goal is **fewer expensive wrong turns**.

## What makes it different

| Layer | What it does |
|---|---|
| Skill discovery | Searches reusable Agent Skills before reinventing workflows |
| Technical research | Prioritizes official docs, source code, maintained examples and real issues |
| Product research | Looks at workflows, competitors, reviews, complaints, pricing and switching reasons |
| Commercial research | Investigates ICP, buying triggers, objections, acquisition and packaging |
| Verification | Triangulates material claims and exposes uncertainty |
| Decision | Rejects weak alternatives and chooses a path |
| Blueprint | Converts evidence into architecture + implementation + GTM |
| Execution discipline | Stops research once enough evidence exists to act |

## Supported tracks

`AGENT` · `WEBSITE` · `SAAS_SOFTWARE` · `AUTOMATION` · `SALES_OFFER` · `SKILL_META`

## Quick start

Clone this repository into a skills directory supported by your agent environment:

```bash
git clone https://github.com/matteuzdev/research-before-build.git
```

Common patterns:

```text
skills/research-before-build/
.agents/skills/research-before-build/
.claude/skills/research-before-build/
```

Then ask your agent to use the skill before a non-trivial build, for example:

> Use research-before-build and design a production-ready Python + Agno receptionist for WhatsApp.

## Example: AI agent

Before coding, the skill drives the agent to investigate current framework primitives, memory/session state, tools, RAG, handoff, observability, channel constraints, data handling, maintained reference implementations and failure modes. It then returns an implementation blueprint.

## Example: website

For a local-business website, the workflow checks search intent, competitor presentation, trust signals, conversion hierarchy, mobile UX, SEO/schema, deployment and measurement before producing code.

## Example: SaaS

For a micro-SaaS, the workflow searches substitutes, competitors, complaints, pricing, customer workflows, acquisition channels, architecture and support burden before selecting the product wedge.

## Repository structure

```text
research-before-build/
├── SKILL.md
├── README.md
├── LICENSE
├── CHANGELOG.md
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── SECURITY.md
├── docs/
│   └── architecture.md
├── references/
│   ├── source-priority.md
│   ├── agent-research.md
│   ├── website-research.md
│   ├── saas-research.md
│   ├── sales-research.md
│   └── validation-checklist.md
├── templates/
│   ├── research-brief.md
│   ├── build-blueprint.md
│   └── evidence-ledger.md
├── examples/
│   ├── agno-human-facing-agent.md
│   ├── local-business-website.md
│   └── micro-saas.md
└── .github/
    ├── pull_request_template.md
    └── ISSUE_TEMPLATE/
```

## Research philosophy

1. **Primary before commentary.** Official docs, specs, APIs and source code carry more weight than generic articles.
2. **Current before familiar.** Fast-changing stacks require current evidence.
3. **Failures matter.** Search issues, limitations and negative evidence—not just success stories.
4. **Market evidence is different from technical evidence.** Treat them separately.
5. **Popularity is not proof.** Stars, likes and search ranking are discovery signals, not validation.
6. **Stop when a decision is justified.** Research should reduce uncertainty enough to act.

## Human-facing agents and identity

The skill encourages natural, concise, context-aware conversational UX. It does **not** instruct agents to impersonate a human or falsely claim human identity. If directly asked about identity or nature, the deployed agent should answer truthfully and follow the product's disclosure requirements.

## Inspirations and credits

This project was informed by patterns from excellent open Agent Skill projects, including:

- **skill-forge** by `bm629/agent-skills`
- **deep-research** by `arjunprabhulal/agent-skills`
- **research-workflow** by `jwynia/agent-skills`
- **research** by `PracticalSwan/agent-skills`
- **deep-research** by `firecrawl/web-agent`

This repository does not copy those skills verbatim. It synthesizes general workflow ideas into a research-to-build orchestration system and adds dedicated product, software, website, sales and agent tracks.

## Roadmap

- [ ] Add installer examples for major agent clients
- [ ] Add an optional `find-skills` helper script
- [ ] Add reference adapters for Python/Agno, Vercel/Next.js and common SaaS stacks
- [ ] Add eval scenarios for research quality and premature-build prevention
- [ ] Add a lightweight source/evidence scoring utility
- [ ] Publish to compatible skill directories and marketplaces

## Contributing

Issues and PRs are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a pull request.

## License

MIT. See [LICENSE](LICENSE).
