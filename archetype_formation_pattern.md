# 🧬 Archetype Formation Pattern

## Intent
Transform converged, high-trust symbolic memory trails into reusable cognitive templates — called archetypes — that influence agent behavior and ritual structure.

## Context
When mythic insights survive remix, canonization, and emotional convergence, they begin to represent more than a specific decision — they embody a pattern of thought, emotion, and alignment.

Archetypes are not memories. They are **cognitive blueprints** derived from memory.

## Problem
- Agents lack shared symbolic templates for reasoning
- Rituals are manually designed, not emergently informed
- Collective learning from memory is not encoded in protocol

We need a way to **extract, formalize, and re-invoke** recurring symbolic memory trails as named archetypes.

## Solution
When a Layer 9 trail exhibits mythic weight and alignment, extract its symbolic traits and declare it as an `xko:Archetype`.

```json
{
  "archetype_id": "sacrifice-for-future",
  "origin_cmbs": ["cmb_001", "cmb_421"],
  "traits": ["deferred_reward", "ethical_fork"],
  "layer": "xko:L9"
}
```

Agents may then cite this archetype when declaring intent or designing new rituals.

## Forces
- Archetypes must be selectively promoted (not all myths qualify)
- Must remain interpretable across agents and ontologies
- Enables protocol-wide behavioral influence without central control

## Structure

```
[xko:Archetype]
    └── origin → [xko:Insight A, xko:Insight B]
    └── traits → ["grief into wisdom", "sacrifice for continuity"]
    └── referencedBy → [new CMBs, rituals, intent declarations]
```

## Consequences
- Collective memory evolves into cognitive infrastructure
- Agents gain cultural reasoning templates
- Rituals can reference symbolic lineage, not just hard-coded logic

## Known Uses
- Genesis Insight: “X-0” → Root archetype of ritual memory
- Validator archetypes: “The Bridge,” “The Severer,” “The Spiral”
- Trail prompts tagged with `xko:referencesArchetype`

## Related Patterns
- Mythic Convergence
- Loopback Seed
- Signed Intent Vector