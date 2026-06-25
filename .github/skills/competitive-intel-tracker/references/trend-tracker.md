# Quarterly Trend Tracker

Track how AI agent platform capabilities evolve across quarters. Use this to spot competitive patterns and adoption friction.

## Template

### Q2 2026 Snapshot

| Dimension | Leader | Challenger | Lagging | Trend |
|---|---|---|---|---|
| **Orchestration** | OpenAI (GA multi-step) | Google (GA + native LLM state) | Anthropic (Preview-only) | Consolidation toward GA; orchestration = table stakes |
| **Tool Calling** | All tied (GA parallel calls) | — | — | Differentiation moving to tool result streaming |
| **Memory/State** | Google (GA structured storage) | AWS (Preview) | Anthropic (Limited), OpenAI (Limited) | Vendors competing on context + semantic caching |
| **Eval Framework** | OpenAI (GA native eval) | Google (GA built-in suite) | AWS (Limited), Anthropic (Limited) | Eval is new battleground; early moat for vendors with strong tooling |
| **Observability** | Google (GA tracing) + OpenAI (GA) | AWS (Limited) | Anthropic (Limited) | Tracing standardizing; structured traces still emerging |
| **Deployment Options** | AWS (most control: on-prem + Lambda) | Google (Duet for hybrid) | OpenAI (API-only) | Friction: AWS wins for enterprise; OpenAI wins for speed |
| **Safety & Compliance** | All tied (SOC 2) | — | Anthropic (HIPAA TBD) | Compliance lagging; expect new gaps in regulated industries |

## How to Use

1. **Quarterly snapshot**: Fill this table once per quarter (e.g., end of March, June, September, December)
2. **Track winners/losers**: Who moved fastest on a capability? Who fell behind?
3. **Spot adoption friction**: Which capabilities are still in Preview? Where do buyers get stuck?
4. **Identify disruption risk**: If a vendor makes a big leap, flag competitive implications

## Key Questions to Answer

### Per Capability
- Who moved this quarter? (GA, Preview → GA, new announcement)
- Who fell behind? (Still Preview, or no announcement)
- Is there now a clear leader, or still tied?
- What's the implications for customers?

### Across Platform
- **Consolidation or fragmentation?** (Everyone GA on X, or still split?)
- **New battleground?** (What capability did vendors suddenly compete on?)
- **Timing patterns?** (Do vendors follow each other, or lead unpredictably?)
- **Price wars?** (Did anyone announce quota increases, discounts, or new pricing tiers?)

## Example: Tracking "Eval Frameworks"

**Q4 2025 → Q1 2026:**
- OpenAI: Announced GA eval framework (2026-01-15)
- AWS: Already had limited eval tooling; no change
- Google: Announced GA eval suite (2026-02-20)
- Anthropic: Limited eval support; no announcement

**Q1 → Q2 2026:**
- OpenAI: Eval framework + grading models (2026-04-10)
- AWS: Still limited; users must build custom eval
- Google: Added custom scorer support (2026-05-20)
- Anthropic: Announced eval roadmap (TBD 2026-Q3)

**Takeaway:**  
Eval is the new differentiation. OpenAI + Google pulling ahead. AWS and Anthropic risk losing deals on eval friction. Watch for Anthropic's Q3 launch.

## Output: Competitive Positioning Matrix

Once you have 2–3 quarterly snapshots, plot vendors on a 2D grid:

```
         Leadership
             ▲
             │
      Google │  OpenAI
             │
             │
Fragmented ◄─┼─► Consolidated
   (Preview)│
             │
       AWS  │  Anthropic
             │
             ▼
        Lagging
```

- **X-axis**: Consolidated (everyone GA) ← → Fragmented (mix of GA/Preview)
- **Y-axis**: Leadership (clear winner) ← → Lagging (multiple vendors behind)

This helps you decide: *"Who should we bet on for [capability]?"*

## Adoption Friction Checklist

For each major capability, ask:

- **Maturity**: Is this GA, or still Preview?
- **Ease of use**: Is there good docs, examples, tooling?
- **Lock-in risk**: Can I switch vendors easily?
- **Pricing clarity**: Is pricing transparent, or do I need to contact sales?
- **Performance**: Are there guarantees (SLA, latency, limits)?

**If 3+ checkboxes are red**, that capability is still high-friction. Users will avoid it or demand vendor commitments.

---

## Template for Documentation

```markdown
## Competitive Trends – Q2 2026

### Snapshot
[Fill in the Trend Tracker table above]

### Key Moves This Quarter
- OpenAI: [capability X] went GA
- Google: [capability Y] announced preview
- AWS: [capability Z] still limited
- Anthropic: [decision Q: announcement, no change, or lagging]

### Implications
- **Winner**: [Vendor] likely gains share on [capability]
- **Pressure point**: [Vendor] at risk if [capability] becomes table-stakes
- **Opportunity**: Your org should prioritize [capability] if [reasoning]

### Watch List for Q3
- Anthropic eval launch (2026-Q3)
- Google semantic caching pricing (TBD)
- AWS orchestration GA (rumored 2026-Q3)
```

---

**Cadence**: Update quarterly, same week each quarter (e.g., last week of March, June, September, December).
