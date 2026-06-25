---
name: competitive-intel-tracker
description: 'Track AI agent platform competitive intelligence across OpenAI, AWS, Google, Anthropic. Collect announcements, compare capabilities, curate datasets for eval, and surface market trends. Use when building market research, evaluating platform fit, or tracking roadmap implications.'
argument-hint: 'Describe timeframe, vendors, focus area (e.g., "Last 14 days, all vendors, agent orchestration + tooling").'
user-invocable: true
---

# Competitive Intelligence Tracker

A bundled workflow for collecting, curating, and analyzing AI agent platform capabilities across the big four (OpenAI, AWS, Google, Anthropic).

## When to Use

- **Market scans**: Weekly or monthly competitive updates for roadmap planning
- **Platform evaluation**: Comparing capabilities before adopting a new platform
- **Feature tracking**: Monitoring specific capabilities (eval, memory, security, pricing)
- **Dataset curation**: Extracting market data for benchmarking or trend analysis
- **Strategic decisions**: Understanding competitive timing and positioning

## Quick Start

1. **Trigger the scan**  
   Invoke via slash command: `/competitive-intel-tracker`  
   Or ask the agent: *"Scan agent platforms—last 14 days, executive brief format."*

2. **Get structured results**  
   Agent returns:
   - Latest updates per vendor with source links
   - Competitive takeaways (3–5 bullets)
   - Watch list (items likely coming next month)

3. **Attach file instructions**  
   Save results to a file matching `*compet*.md`, `*market*.md`, or `*intel*.md`  
   File instructions will auto-load best practices for structuring and updating

4. **Curate datasets**  
   Use the [capability matrix template](./references/capability-matrix.md) to extract structured data for eval or benchmarking

## Workflow

### Step 1: Define Your Research Question
- Timeframe: last 7/14/30 days or custom range
- Vendors: all four, or specific set
- Focus: agent orchestration, tool-calling, memory, eval, deployment, security, pricing?

### Step 2: Collect
Use `@AI Agent Platform Competitive Intel` agent to gather latest announcements from official sources, with media fill-in where gaps exist.

### Step 3: Structure
Organize findings into:
- **Vendor updates** (1 paragraph each)
- **Capability deltas** (new vs. changed vs. deprecated)
- **Strategic implications** (who moved on what, adoption risk)
- **Next-month watch list**

### Step 4: Curate (Optional)
Extract findings into a structured capability matrix for:
- Benchmarking platform fit
- Eval dataset seeding
- Trend analysis across quarters

### Step 5: Frame for Microsoft Sellers (Optional but Recommended)
For each competitor update, add a "Why It Matters to Microsoft Sellers" section:

**For each vendor announcement, analyze:**
- **Direct comparison to Azure/Microsoft offerings**: How does this capability compare to what Microsoft provides?
- **Customer impact**: Would this capability influence a customer's platform choice?
- **Sales friction points**: Does this create a gap customers might perceive? Or does it reinforce Microsoft's positioning?
- **Proof points**: Does this validate a Microsoft strategy, or does it suggest Microsoft is behind on something?
- **Deal implications**: Could this announcement delay, accelerate, or block a Microsoft deal? Why?
- **Messaging opportunity**: What should sellers say about this when customers bring it up?

**Example frame:**
```
Update: [Vendor] announced [capability]

Why It Matters to Microsoft Sellers:
- **Customer perception**: Customers may view this as [advantage/threat/differentiation for competitor]
- **vs. Microsoft**: Azure AI [does/doesn't] offer equivalent; the gap is [specific detail]
- **Seller talking point**: "Vendor X is strong on [capability], and we match them on [specific], 
  but our advantage is [Microsoft differentiator]"
- **Deal risk**: ⚠️ High risk if customer prioritizes [this capability] 
  → Recommend: [specific Azure positioning or workaround]
```

## Reference Materials

- [Capability Matrix Template](./references/capability-matrix.md) — standardized comparison structure
- [Source Guidelines](./references/source-guidelines.md) — how to validate and cite sources
- [Trend Tracker](./references/trend-tracker.md) — quarterly capability trend patterns
- [Microsoft Seller Guide](./references/seller-guide.md) — how to frame competitor announcements for sales conversations + talking points

## Output Formats

### Executive Brief (Default)
Timeframe + vendor updates + 3–5 bullets + watch list. ~500 words, scannable in 2 minutes.

### Executive Brief + Seller Context (Recommended for Sales Teams)
Same as above, but each vendor update includes a "Why It Matters to Microsoft Sellers" subsection:
- Direct comparison to Azure/Microsoft
- Sales friction points or proof points
- Recommended seller talking points
- Deal risk assessment (low/medium/high)

### Capability Matrix
Rows = capabilities, columns = vendors, cells = status (GA/preview/absent) + date + source.

### Trend Deep Dive
Quarterly capability evolution + competitive positioning + adoption friction points.

### Sales Pitch Brief
Designed for field sellers: competitor announcements → Azure counter-positioning + talking points + deal strategy per scenario.

## Tips

- **Keep it sourced**: Every claim needs a URL; link from source directly so readers can verify
- **Identify patterns**: Is vendor X consistently faster on orchestration? Stronger on safety? Track across quarters
- **Flag conflicts**: If sources disagree on capability status, call it out and avoid definitive claims
- **Timeframe consistency**: Default to last 14 days; call out when older sources are intentional (e.g., "GA status as of Q2 2026")

## Seller-Focused Tips

### Framing Competitor News for Sales Impact

1. **Ask the Deal Question First**  
   Before analyzing a capability: "Does this announcement change how we position Microsoft to this customer segment?"  
   If no → brief mention. If yes → deep seller context.

2. **Map to Azure/Microsoft Equivalent**  
   Every competitor announcement should trigger: "Do we have this? If not, when?"
   - **If we're ahead**: Articulate the Microsoft advantage
   - **If tied**: Emphasize what differentiates (speed, price, support, integration)
   - **If behind**: Identify the gap + timeline to close it + interim workaround

3. **Call Out Deal Risk**  
   For each update, assess:
   - **Low risk**: Competitor announced something we already have or don't compete on
   - **Medium risk**: Competitor closed a gap; customers may notice but won't change deals yet
   - **High risk**: ⚠️ Competitor has material advantage; expect customer questions; have a response ready

4. **Provide Seller Talking Points**  
   Example format:
   ```
   Customer brings up: "AWS just announced web search in agents"
   Seller says: "Great timing—that's a capability we've had for 6 months via Azure AI Search integration. 
   Plus, here's where we differ: [specific Azure advantage]"
   ```

5. **Track Competitive Positioning Over Time**  
   - Is a vendor suddenly aggressive on a capability you thought was Microsoft-only?
   - Is a competitor taking months to launch something you thought was table-stakes?
   - Update your pitch: "This tells us customers are prioritizing [X]; we're already strong there."

### When to Escalate Competitor News

Flag updates for immediate seller briefing if:
- Competitor announced GA of a capability in your current ACP (Active Compete Plan)
- A customer-specific deal might be affected
- Requires new messaging or talking points
- Suggests a shift in competitive positioning (e.g., vendor moving into a new market)

## Integration with Roadmap

Use results to:
1. Decide which platforms to prioritize for internal eval
2. Identify capability gaps vs. competitors
3. Time feature launches relative to vendor momentum
4. Benchmark pricing and quota changes

## For Sales Teams & Solution Architects

Use competitive scans to:
1. **Prepare for customer conversations**: Understand competitor announcements before customers ask
2. **Build deal strategies**: "If customer cares about [capability], here's why Azure is the right choice"
3. **Update battle cards**: Refresh your competitive positioning statements quarterly
4. **Brief account teams**: Weekly or bi-weekly sync on "What competitors announced + what to say"
5. **Identify upsell/expansion**: Competitor moves often reveal customer priorities you should address in current accounts

### Seller Briefing Template

When sharing competitive scans with sales teams, frame it:

```markdown
## Week of [Date] – Competitor Updates Worth Knowing

### Quick Summary
Competitor X announced [capability]. **Deal risk: [Low/Medium/High]**

### Why It Matters to You
[Direct impact to your selling motion or current deals]

### What to Say If a Customer Mentions This
"[Customer concern] → [Microsoft positioning]"

### Questions to Ask Your Account Team
- Do any of your current opportunities prioritize [this capability]?
- If yes, should we adjust the pitch or timeline?
```

---

**Next steps:**  
Once you have a competitive scan, consider:
1. Creating a [continuous-eval](./references/continuous-eval-setup.md) pipeline to track how platform capabilities impact your eval results.
2. For sales teams: Convert this week's scan into a brief battle card or seller briefing for your account teams.
3. Track which competitor announcements actually affect your deals—use that data to refine future scans to focus on your key competitive battlegrounds.
