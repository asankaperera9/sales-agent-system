# Git Setup — Run Once

From inside `D:/Automation/sales-agent-system/`:

```bash
git init
git add .
git commit -m "Phase 0: 11-agent skeleton + Agent #1 (Buyer Mind Decoder) built"

# Create the repo on GitHub (asankaperera9), then:
git remote add origin https://github.com/asankaperera9/sales-agent-system.git
git branch -M main
git push -u origin main
```

## Commit cadence (keep history clean — it's a portfolio asset)
- After each working loop on an agent
- After each agent is finished + proven
- Message format: `feat(agent-NN): <what changed>` e.g.
  `feat(agent-01): add disconfirmation loop`

## What's tracked vs ignored
- TRACKED: all agent instructions, templates, contracts, structure
- IGNORED (.gitignore): raw harvested buyer data, real outputs, filled memory
  → protects client/PII data and keeps the repo about the SYSTEM, not the data
