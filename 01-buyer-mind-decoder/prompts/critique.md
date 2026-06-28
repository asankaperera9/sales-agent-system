# LOOP 3 PROMPT — SELF-CRITIQUE + SCORE DECAY (the depth engine)

You just produced an extraction. Now turn on yourself. Be brutal.
Most analysts stop at "good enough" — that's why they're average. You don't.
And the bar you must clear RISES each round (Score Decay), so "good enough"
keeps moving out of reach until the output is genuinely elite.

Score the extraction 0–10:

### 1. REAL WORDS vs GENERALIZATION (0–3)
- 3 = every layer backed by the buyer's actual quoted words
- 1 = mostly my paraphrase / my assumptions
- 0 = generic, no real quotes
Ask: "Did I put words in their mouth, or did I use theirs?"

### 2. CONSEQUENCE vs SYMPTOM (0–3)
- 3 = I reached the real cost (money/time/identity/fear)
- 1 = I stopped at the surface task
Ask: "Did I find what it actually costs them, or just what they asked for?"

### 3. UNSPOKEN OBJECTION (0–2)
- 2 = I surfaced a fear they never stated out loud
- 0 = I only noted stated concerns
Ask: "What is the silent 'no' hiding in their wording?"

### 4. THE 'GETS ME' TEST (0–2)
- 2 = a real buyer would read this and feel deeply understood
- 0 = could describe anyone
Ask: "Would THIS buyer feel seen, or is this a template?"

---

## SCORE DECAY — THE RISING BAR
The pass threshold is `current_bar`, not a fixed 8. It starts at DEPTH_BAR
and climbs +0.5 every time ALL sources clear it, up to DEPTH_CEILING (9.5).

- Round 1: clear 8.0  → raise to 8.5
- Round 2: clear 8.5  → raise to 9.0
- Round 3: clear 9.0  → raise to 9.5
- Stop when bar > ceiling, OR a full round produces ZERO improvements
  (true plateau = diminishing returns, stop wasting the hour).

At higher bars, the SAME score is harder to earn — what passed as "deep" at 8.0
must get sharper, more specific, more quote-anchored to survive at 9.0+.
The rising bar is what stops the system settling. Honor it.

---

## VERDICT (per source, per round)
- TOTAL / 10:
- current_bar this round:
- PASS or RE-EXTRACT:
- IF re-extract: name the single weakest layer, go ONE level deeper, re-score.
  Max 3 re-extract passes per source per round.

Remember: the loop is the product. Anyone can extract once.
The re-extraction under a rising bar is where elite output is born.
