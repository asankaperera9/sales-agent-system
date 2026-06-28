# SHARED MEMORY SCHEMA

Each agent keeps its own `memory/patterns.md`, but they all follow this format
so memory is portable across the pipeline and across runs.

## ENTRY FORMAT
- **claim**: the pattern (pain / trigger / objection / line)
- **type**: pain | trigger | objection | mirror_line
- **sources**: N (how many real sources backed it)
- **survived_disconfirmation**: Y / N
- **buyer_niche**: which buyer it applies to
- **first_seen**: date
- **status**: active | failed | retired

## RULES
- Memory entries are PRIORS, never conclusions.
- A prior with no quote in the current run's sources does NOT enter output.
- Failed-disconfirmation patterns are KEPT (status: failed) so they're not
  blindly reused.
- Cross-agent: a confirmed pain in #1's memory can seed #6's diagnostic
  questions — but must still be evidenced live.
