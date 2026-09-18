# Architecture

Research Before Build is intentionally a **router + evidence pipeline**, not a knowledge dump.

```text
User request
   │
   ├─ classify domain + risk
   │
   ├─ discover reusable skills
   │
   ├─ build research questions
   │
   ├─ gather technical + market evidence
   │
   ├─ resolve contradictions
   │
   ├─ make explicit decision
   │
   └─ emit blueprint → build → validate
```

## Design goals

- portable across agent environments
- current-source aware
- decision-oriented, not report-oriented
- explicit about uncertainty
- commercially aware when the project is meant to be sold
- modular enough to extend without bloating `SKILL.md`

## Separation of concerns

`SKILL.md` owns orchestration.

`references/` owns track-specific research checklists.

`templates/` owns reusable output structures.

`examples/` demonstrates intended behavior without becoming mandatory implementation guidance.

## Research stopping condition

Stop when:

1. the material unknowns are bounded,
2. the chosen approach has stronger evidence than realistic alternatives,
3. major risks are known,
4. a concrete next action is available.

More links do not automatically improve a decision.
