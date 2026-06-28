# Sales Agent System — 11-Agent Psychological Pipeline

An agentic system that walks a buyer from **stranger → closed deal**, one
psychological stage at a time. Each stage is its own looping agent. Together
they form one pipeline: each agent's OUTPUT is the next agent's INPUT.

Built with Claude Code (Opus 4.8). Runs locally — these are agent instructions
+ structured files, not a web app. Deploy only when wrapped in an app later.

---

## THE GOLDEN RULE (read this first)
> **Build to 11. Finish 1 at a time.**
> The folder holds all 11 agents so the architecture is locked. But only ONE
> agent gets finished before it earns its keep — i.e. produces real output that
> helps win or sharpen a real Upwork deal. This is a deliberate guard against
> the 47-unfinished-folders pattern. The skeleton is permission to plan, not to
> build everything at once.

---

## THE 11 AGENTS (the psychological path to a closed deal)

| # | Agent | Job | Eats | Produces |
|---|-------|-----|------|----------|
| 01 | **Buyer Mind Decoder** ✅ | Decode buyer psychology at elite depth | Raw buyer language | Buyer Psychology Profile |
| 02 | Prospect Finder | Find buyers who match the profile | #1 profile | Scored prospect list |
| 03 | Authority Builder | Value-first content that attracts | #1 + #2 | Publish-ready content |
| 04 | Conversation Opener | Open with curiosity, not a pitch | #1 + a prospect | Personalized opener |
| 05 | Lead Qualifier | Mutual-fit check | reply to #4 | Qualify verdict |
| 06 | Pain Diagnoser | Make the real cost vivid | qualified lead | Diagnostic Qs + real cost |
| 07 | Solution Positioner | Sell the transformation | #6 + #1 | Tailored positioning |
| 08 | Objection Handler | Dissolve the silent "no" | #1 + state | Pre-emptive responses |
| 09 | Momentum Creator | Clear next step + real urgency | #7/#8 | Next-step proposal |
| 10 | Closer | Ask directly | #9 | Direct close message |
| 11 | Follow-Up Engine | Persist without begging | any stall | Value follow-up sequence |

✅ = built. The rest are STUBS with locked input→output contracts.

---

## PHASE PLAN (complexity removed by sequencing)

- **Phase 0 — Skeleton** ✅ (this) — master folder, 11 contracts, git, Agent #1 in.
- **Phase 1 — Prove #1** — run Buyer Mind Decoder on real Upwork data; produce
  2–3 profiles; use one in a real proposal. Gate: did it sharpen the pitch?
- **Phase 2 — Build #2 (or the Pitch Composer)** — only after #1 proves.
  Shortest path to money may be jumping to a pitch-writer that eats #1's output.
- **Phase 3+ — Fill the pipeline** — one agent at a time, each proven before next.
  Some agents may merge or die. That's healthy complexity removal.

---

## STRUCTURE
```
sales-agent-system/
├── README.md                 ← this file (the master plan)
├── pipeline/contract.md      ← the shared input→output data contract
├── shared/
│   ├── memory/schema.md      ← cross-agent memory format
│   └── templates/            ← reusable templates
├── 01-buyer-mind-decoder/    ← BUILT
│   ├── agent_loop.md, prompts/, templates/, memory/, data/, output/
└── 02-…11-…/                 ← STUBS (STUB.md = contract + build checklist)
```

## RUNNING (Claude Code)
1. `cd` into the agent you're working (start with `01-buyer-mind-decoder/`)
2. Use its `agent_loop.md` as the agent instructions
3. Feed inputs per the pipeline contract; review `output/`
4. Commit after each working loop

## FOCUS NOTE
This system lives in the **1hr/day Upwork cash track**. csoft-erp + the shop
demo remain #1. This is a real portfolio asset — and a real temptation to
over-build. Honor the Golden Rule.
