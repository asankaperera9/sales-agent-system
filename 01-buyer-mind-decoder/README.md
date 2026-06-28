# Buyer Mind Decoder — Agent #1 (v2)

The first agent in your agentic sales system. Decodes a buyer's psychology
from raw, real-world language with elite depth via a self-critique loop.

## Why this is not average
99% of "buyer research" tools do ONE pass and output generic personas.
This agent **loops on itself** — extracts, attacks its own conclusions, judges
depth against a RISING bar, tests its own output, and remembers across runs.
The loops are the product. The extraction is the easy part.

## The Loops
- **0. Load Memory** — read past patterns as priors (gets smarter each run)
- **1. Harvest** — gather raw verbatim language (+ diversity guard)
- **2. Extract** — pull the 4 psychological layers per source
- **3. Self-Critique + Score Decay** ⭐ — judge depth against a RISING bar
- **3.5 Disconfirmation** — attack each headline claim before trusting it
- **4. Synthesize** — aggregate into one Buyer Psychology Profile
- **5. Output-Test** — simulate the buyer; keep only pitch lines they'd answer
- **6. Write Memory** — make the next run smarter

## Run order (Claude Code)
1. Drop raw buyer posts into `data/raw/` (≥3 source types)
2. Use `agent_loop.md` as the agent's instructions
3. Agent loops until depth + disconfirmation + output-test all pass
4. Review final `output/profile.md`
5. `memory/patterns.md` auto-grows each run

## Files
- `agent_loop.md`        — the brain (all loops, v2)
- `prompts/critique.md`  — Loop 3 rubric + Score Decay rising-bar rules
- `templates/extraction.md` — per-source extraction template
- `templates/profile.md` — final one-page deliverable
- `memory/patterns.md`   — persistent cross-run memory
- `data/raw/`            — drop raw buyer posts here
- `data/extracted/`      — per-source structured extractions
- `output/`              — final Buyer Psychology Profile

## The 1-hour discipline (Upwork track)
One real source, fully looped, per session beats ten skimmed.
Don't perfect — extract. Ship one entry per session. csoft-erp stays #1.
