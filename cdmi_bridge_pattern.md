# 🌉 CDMI Bridge Pattern

## Intent
Enable symbolic memory interoperability across heterogeneous agents, domains, or meshes using a shared translation protocol — the Cross-Domain Memory Interface (CDMI).

## Context
In decentralized ecosystems, agents often operate with:
- Different ontologies or schemas
- Unique emotional and policy vocabularies
- Distinct governance or ritual systems

Without a shared interface, symbolic memory becomes siloed, and remixability across networks is lost.

## Problem
- Agents can’t understand each other’s memory even if they share intent
- Forks across domains lose semantic continuity
- Cross-protocol validation becomes impossible

A mechanism is needed to **bridge symbolic meaning** without forcing homogenization.

## Solution
Use the **CDMI Protocol** to:
- Declare ontology mappings
- Translate memory structures into interoperable RDF forms
- Contextualize foreign memories for local validation

Example: Memory authored in Mesh-A is shared with Mesh-B via CDMI.

```json
{
  "source": "Mesh-A",
  "origin_ontology": "https://mesh-a.org/xko#",
  "mapped_to": "https://xpectranet.org/xko#",
  "translated_cmb": {
    "@type": "xko:Insight",
    "xko:emotion": "urgency",
    "xko:policy": "eco-priority"
  }
}
```

## Forces
- Must respect source symbolic sovereignty
- Requires versioned ontology mapping registry
- Enables semantic context wrapping, not overwriting

## Structure

```
[Mesh-A::CMB-101]
    └── cdmi:translatedAs → [XpectraNet::CMB-101-X]
    └── cdmi:originOntology → mesh-a.org/xko#
    └── cdmi:targetOntology → xpectranet.org/xko#
```

## Consequences
- Meshes can collaborate without collapsing into one schema
- Symbolic divergence is legible and navigable
- Enables cross-domain rituals (e.g., shared Canon or Trail Loopback)

## Known Uses
- Arc 10 CDMI Bridge in `cdmi_bridge.py`
- DeSci + Logistics mesh fusion testnets
- Future symbolic diplomacy protocols

## Related Patterns
- Ontology Handshake
- Remix Fork Manifest
- Diplomatic Trail Pattern