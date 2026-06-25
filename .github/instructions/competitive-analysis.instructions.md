---
description: "Use when analyzing, tracking, or updating competitive intelligence on AI agent platforms. Auto-attached to files matching market research, competitor scan, or intelligence patterns. Helps structure market data, call the AI Agent Platform Competitive Intel agent, and synthesize cross-vendor comparisons."
name: Competitive Intelligence Guidelines
applyTo: ["**/*compet*.md", "**/*market*.md", "**/*intel*.md", "**/*scan*.md"]
---
# Competitive Intelligence Guidelines

## Use Case
You are aggregating or updating competitive intelligence on AI agent platforms (OpenAI, AWS, Google, Anthropic). Your goal is to produce structured, sourced, scannable market data.

## Process

1. **Invoke the Agent**  
   Use `@AI Agent Platform Competitive Intel` with a clear timeframe and focus:
   - *"What launched this week in agent orchestration?"*  
   - *"Compare tool-calling capabilities across the big four."*  
   - *"Market scan: last 14 days, quick executive brief."*

2. **Structure Results**  
   Organize findings into these sections:
   - **Timeframe & Sources** (dates + official vs. media)
   - **Vendor Updates** (one paragraph per: OpenAI, AWS, Google, Anthropic)
   - **Competitive Takeaways** (3–5 bullets with implications)
   - **Watch This Month** (what's likely coming next)

3. **Validate Sources**  
   - Every claim must cite at least one URL
   - Mark each source: `[official]` or `[media]`
   - If sources conflict, flag the discrepancy instead of picking one

4. **Cross-Check Against Repo History**  
   Look for patterns:
   - Is this a known capability or genuinely new?
   - Does it affect your current platform roadmap?
   - Any timing implications vs. competitors?

## Output Format

```markdown
## [Date Range] AI Agent Platform News 

### Timeframe & Sources
Last 14 days, official sources + trusted media.

### Updates
- **OpenAI**: [capability shift] [source](https://...) 
- **AWS**: [capability shift] [source](https://...)
- **Google**: [capability shift] [source](https://...)
- **Anthropic**: [capability shift] [source](https://...)

### Competitive Takeaways
- [Implication 1]
- [Implication 2]
- [Implication 3]

### Watch This Month
- [Item 1]
- [Item 2]
```

## Key Principles
- **No invented dates or claims** — if you're not certain, say "source not found"
- **Favor official channels** — docs, blogs, changelogs, then media
- **Contextualize changes** — so vs. what? GA or preview?
- **Link every claim** — readers should be able to verify in 10 seconds
