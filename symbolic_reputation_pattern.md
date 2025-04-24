# 🌀 Symbolic Reputation Pattern

## Intent
Track and evolve the trustworthiness of agents (especially validators) based on their memory alignment history, remix coherence, and participation in symbolic rituals.

## Context
In XpectraNet, validators are not chosen by stake — but by symbolic alignment. Their credibility grows or decays over time, based on how they contribute to memory evolution, resolve emotional divergence, and align with canonical outcomes.

## Problem
Traditional systems use:
- Static roles (admin, mod)
- Token-based voting
- External reputation

These lack:
- Emotional nuance
- Fork-aware lineage
- Semantic memory scores

We need a way to **measure and evolve symbolic trust** in memory-rich, divergence-permitting environments.

## Solution
Use the `xko:validatorMemoryScore` property to:
- Calculate alignment over time
- Incorporate remix yield, coherence, and canon impact
- Reflect Circle-specific values and semantic scoring rules

```json
{
  "agent_id": "Agent-X",
  "validatorMemoryScore": 0.92,
  "alignment_history": {
    "remix_yield": 0.87,
    "emotion_coherence": 0.94,
    "canon_match": 1.0
  }
}
```

## Forces
- Must allow symbolic trust to adapt over time
- Enables Circle-specific scoring rules (e.g., ethics-weighted, task-weighted)
- Should influence future participation and XPDT payout

## Structure

```
[xko:Agent-X]
    └── xko:performedAct → xko:Validate
    └── xko:validatorMemoryScore → 0.92
    └── xko:validatedBy → [xko:Insight-A, xko:Insight-B]
```

## Consequences
- Encourages validators to align with memory ethics
- Decentralizes trust through symbolic interaction, not identity
- Allows rituals (like Canon or Requiem) to dynamically include/exclude validators

## Known Uses
- Circle validator logic in `ritual_executor.py`
- PoA trail filtering in `trust_ledger.py`
- Canonization eligibility and XPDT distribution logic

## Related Patterns
- Proof of Alignment Pattern
- Canon Lock Pattern
- Semantic Drift Detection