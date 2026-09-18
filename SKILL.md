---
name: research-before-build
description: Research-first orchestration skill for building and selling AI agents, websites, SaaS/software, automations, and digital offers. Use before architecture, coding, prompting, stack selection, or go-to-market whenever current docs, existing skills, competitors, market evidence, implementation patterns, or source validation could materially change the solution.
license: MIT
version: 1.0.0
compatibility: ChatGPT, Claude Code, Codex, Gemini CLI, GitHub Copilot, Cursor, and other SKILL.md-capable agents
metadata:
  category: research-orchestrator
  mode: research-to-decision
  author: Hianto Mateus / community contributors
---

# Research Before Build

> **Find before inventing. Verify before deciding. Blueprint before building. Evidence before selling.**

This skill is a research-first orchestration layer for non-trivial product work. It turns an ambiguous request into a bounded research plan, searches for reusable skills and authoritative references, validates findings, and converts them into an execution-ready blueprint.

## Activate when

Use this skill when creating, designing, architecting, improving, comparing, selling, or choosing technology for:

- AI agents, assistants, multi-agent systems, voice agents, SDRs, support agents, receptionists and copilots
- websites, landing pages, ecommerce, local-business sites and web apps
- SaaS, micro-SaaS, internal software, APIs, dashboards, CRMs and automations
- digital products, services, offers, acquisition systems, outbound flows, pricing and positioning
- prompts, agent skills, reusable workflows, tools, memory, RAG, observability and deployment

Do not use the heavyweight workflow for trivial facts, tiny edits, or quick sketches where current research would not materially change the outcome.

## Core rule

Research only enough to make a decision.

Every research action must help answer one or more of:

1. What should we build?
2. How should we build it?
3. What should we reuse instead of reinvent?
4. What can fail technically, legally, commercially, or operationally?
5. How will users adopt, buy, or use it?
6. What is the smallest evidence-backed next action?

## Pipeline

### 0 — Classify

Choose one or more tracks:

- `AGENT`
- `WEBSITE`
- `SAAS_SOFTWARE`
- `AUTOMATION`
- `SALES_OFFER`
- `SKILL_META`

Extract outcome, audience, constraints, budget, existing stack, risk level and production expectations.

### 1 — Find existing skills first

Search, in order when available:

1. local/project skills
2. official skill registries and marketplaces
3. skills.sh and similar indexes
4. GitHub repositories containing `SKILL.md`
5. framework/vendor examples and templates

For each candidate record:

- name and source
- trigger/use case
- strongest reusable idea
- assumptions/dependencies
- freshness/maintenance signal
- license if relevant
- adopt, adapt, or reject

Use third-party skills as source material. Do not silently copy them verbatim.

### 2 — Sharpen the research question

Turn the request into 3–7 decision questions.

Example for a Python + Agno customer-facing agent:

- What is the current recommended architecture?
- Which memory, session and knowledge primitives are first-party?
- How are tools, retries, guardrails, handoffs and observability handled?
- What patterns produce natural conversation without deceptive human impersonation?
- Which maintained reference implementations exist?
- What channel/data/privacy constraints apply?
- What is the simplest production architecture that meets the goal?

### 3 — Build the source map

Default priority:

1. official documentation, specs, source code and first-party APIs
2. maintained official examples and repos
3. reputable technical references and standards
4. strong independent benchmarks and case studies
5. GitHub issues/discussions for implementation friction
6. community discussions/reviews for experience signals
7. generic SEO content only for discovery

For market/sales research also use:

- competitor pricing/product pages
- customer reviews and complaint patterns
- job posts and implementation requests
- communities and marketplaces
- ad libraries and public campaigns when relevant

### 4 — Search by angle

Do not use one giant query. Cover:

- official/current
- implementation/examples
- alternatives/comparison
- failures/issues/limitations
- market/customer/pricing
- skills/templates

### 5 — Extract evidence

For each material claim capture:

- claim
- source
- source type
- date/freshness
- precise evidence or paraphrase
- confidence
- decision implication
- contradictions/gaps

Confidence:

- **High** — primary source or 3+ credible sources agree
- **Medium** — 2 credible independent sources agree
- **Low** — one source, stale evidence, or meaningful conflict

Popularity is not proof.

### 6 — Resolve conflicts

When sources disagree:

1. prefer primary/current evidence
2. check version differences
3. identify different scale/use-case assumptions
4. expose unresolved uncertainty
5. do not average incompatible recommendations

Reject patterns that are outdated, abandoned, demo-only when production is required, insecure without evidence, or commercially attractive without user evidence.

### 7 — Produce the blueprint

The research phase must end with:

- problem and target outcome
- chosen approach
- rejected alternatives and why
- architecture/flow
- stack/dependencies
- implementation phases
- risks and mitigations
- validation tests
- commercial model when relevant
- one next action

## Track modules

### AGENT

Investigate as relevant:

- framework version and official primitives
- model/provider abstraction
- tools/tool calling
- session state and persistent memory
- knowledge/RAG
- prompt/instruction architecture
- structured outputs
- guardrails
- human handoff
- failure recovery and idempotency
- latency/cost
- observability/tracing/evals
- deployment/runtime
- secrets/data handling
- channel integration
- conversation UX

For customer-facing agents, optimize for natural, concise, context-aware conversation. Never instruct the agent to falsely claim it is human. If directly asked about identity, answer truthfully.

### WEBSITE

Research:

- conversion goal and traffic source
- competitor/reference sites
- information architecture
- copy and trust signals
- mobile-first UX
- accessibility
- performance/Core Web Vitals
- SEO and structured data
- AEO/GEO when relevant
- analytics and conversion events
- forms, WhatsApp and booking flows
- CMS/admin need
- hosting, deployment and domain
- maintenance model

Start from conversion job and content hierarchy, not visual style alone.

### SAAS_SOFTWARE

Research:

- ICP / job-to-be-done
- painful current workflow
- competitor matrix
- review mining: complaints, missing features, switching reasons
- willingness-to-pay and substitutes
- activation moment
- retention loop
- onboarding
- pricing/packaging
- architecture and data model
- auth/roles/permissions
- integrations
- billing
- observability
- security/privacy/compliance
- support burden
- acquisition channel

Avoid feature-list cloning.

### AUTOMATION

Research:

- trigger
- source of truth
- actions
- idempotency
- retries
- rate limits
- failure queue
- audit trail
- approval gates
- secrets/auth
- webhook vs polling
- cost per run
- monitoring

### SALES_OFFER

Research:

- ICP and buying trigger
- painful before-state
- desired outcome
- alternatives/substitutes
- proof
- objections
- price anchors
- competitor packaging
- acquisition channels
- sales cycle
- fulfillment cost
- recurring revenue opportunity
- risk reversal

Do not claim validation from anecdotal examples alone.

### SKILL_META

When creating or improving another skill:

- search existing skills first
- identify reusable procedures and gaps
- synthesize, do not blindly merge
- keep the resulting skill focused and portable
- move long detail into `references/`
- include activation and non-activation rules
- include tool-independent fallbacks
- credit inspirations in README/research notes

## Fast mode vs deep mode

### Fast mode

Use for bounded low-risk builds.

Minimum:

- one skill search
- 2–4 strong sources
- one implementation reference
- explicit blueprint

### Deep mode

Use for production systems, meaningful investment, unfamiliar stacks, security-sensitive work, or major commercial decisions.

Minimum:

- 3–5 research angles
- primary documentation
- implementation evidence
- failure/limitation evidence
- market evidence when commercial
- conflict resolution
- evidence ledger
- architecture decision record

## Quality gate

Do not move to build until:

- [ ] request classified
- [ ] existing skills/templates searched where appropriate
- [ ] current primary sources checked for fast-changing tech
- [ ] at least one failure/limitation search completed for non-trivial builds
- [ ] material claims have evidence
- [ ] conflicts resolved or explicitly marked unresolved
- [ ] chosen approach justified against at least one realistic alternative
- [ ] blueprint contains one concrete next action

## Output contract

Default output:

1. **Decision**
2. **Evidence**
3. **Blueprint**
4. **Risks**
5. **Next action**

For long research tasks also produce an evidence ledger and source map.

Do not dump every search result onto the user.

## ADHD-friendly mode

When reduced cognitive load is useful:

- keep one active implementation objective
- park tangents
- show stage: `Research → Decision → Blueprint → Build → Validate`
- give one next action unless a full roadmap is requested
- avoid endless option lists
- prefer a default once evidence is sufficient

## Tool fallbacks

- no skills marketplace → search GitHub for `SKILL.md` + domain keywords
- no web search → use available official docs/source and state freshness limits
- no GitHub connector → use public GitHub web access
- no browser → rely on text/API sources
- no parallel agents → execute research angles sequentially
- no persistent files → return blueprint and evidence ledger inline

Never pretend a source was checked when it was not.
