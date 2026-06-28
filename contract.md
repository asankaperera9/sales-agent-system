# PIPELINE CONTRACT — How Agents Hand Off

The system works only if every agent's OUTPUT cleanly becomes the next agent's
INPUT. This file is the source of truth for those handoffs. Change a contract
here BEFORE changing an agent, never after.

## HANDOFF FORMAT
Every agent reads/writes structured markdown in its own `output/`. The next
agent reads from the previous agent's `output/`. No agent invents data the
contract doesn't supply.

## THE CHAIN
```
raw buyer language
   │
   ▼
[01 Buyer Mind Decoder] ──► output/profile.md
   │  (top pains, identity, trigger map, objection map, mirror-language)
   ▼
[02 Prospect Finder] ──► output/prospects.md
   │  (scored real prospects + where found + fit reason)
   ▼
[03 Authority Builder] ──► output/content.md
   ▼
[04 Conversation Opener] ──► output/opener.md   (per prospect)
   ▼
[05 Lead Qualifier] ──► output/qualified.md
   ▼
[06 Pain Diagnoser] ──► output/diagnosis.md
   ▼
[07 Solution Positioner] ──► output/positioning.md
   ▼
[08 Objection Handler] ──► output/objection-responses.md
   ▼
[09 Momentum Creator] ──► output/next-step.md
   ▼
[10 Closer] ──► output/close.md
   ▼
[11 Follow-Up Engine] ──► output/followup-sequence.md
```

## SHARED KEYS (every profile carries these so downstream agents can rely on them)
- `buyer_niche`
- `top_pains[]`        (each with evidence quotes)
- `identity_gap`
- `trigger_map`        (#1 trigger + supporting)
- `objection_map`      (#1 silent objection + others)
- `mirror_language[]`  (opener / pain-mirror / trust / close lines)

## RULE
If you add a field an agent needs, add it to the SHARED KEYS here first, then to
Agent #1's profile template, so it flows down the whole chain.
