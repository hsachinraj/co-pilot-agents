---
name: Get Latest Vendor News
description: "Fetch latest news and announcements from AI agent platforms (OpenAI, AWS, Google, Anthropic) within a timeframe. Returns detailed breakdown with competitive implications and seller talking points. Use when tracking market updates or preparing customer conversations."
argument-hint: "Vendors (e.g., 'all' or 'OpenAI, AWS'), timeframe (e.g., '7 days', '2 weeks'), optional focus (e.g., 'agent orchestration', 'pricing')."
agent: "AI Agent Platform Competitive Intel"
tools: [web, search]
---

Get the latest news and announcements from AI agent platforms within the requested timeframe.

## Your Task
Gather recent news, product announcements, and updates from: google and OpenAI  
Timeframe: Last 30 days 
Focus area (optional): {{focus_area}}

## Requirements
- **Use official sources**: Vendor docs, blogs, release notes, product pages
- **Validate dates**: Include publication/announcement dates for all items
- **Organize by vendor**: Clear section per vendor
- **Cite sources**: Include direct links for verification (readers should verify in <10 seconds)
- **Distinguish status**: Mark updates as GA / Preview / Roadmap / Announcement
- **Include seller context**: For each update, explain why it matters to Microsoft positioning

## Output Format (Detailed Breakdown)
Return comprehensive analysis with these sections:

1. **Timeframe & Source Quality**: "Last {{timeframe}}, official sources"

2. **Vendor Updates** (one section per vendor):
   - What was announced (1-2 sentences)
   - Status: GA / Preview / Roadmap / Announcement
   - Release/announcement date
   - Source link(s)
   - **Why It Matters to Microsoft Sellers**:
     - How does this compare to Azure/Microsoft offerings?
     - Sales friction point or proof point?
     - Deal risk: Low / Medium / High
     - Recommended seller talking point

3. **Competitive Takeaways**: 4-5 bullets on strategic implications and market trends

4. **Deal Risk Assessment**:
   - Which vendors moved on key capabilities?
   - Likely customer questions and recommended responses
   - Suggested positioning per scenario

5. **Watch List**: What's likely coming from each vendor in the next 2-4 weeks

## Constraints
- DO NOT invent announcements, dates, or metrics
- DO NOT mix old news with current timeframe
- DO NOT provide comparisons without sourcing each claim
- If data is missing, state "No reliable recent source found" rather than guessing
- For selling context, reference Azure AI and Microsoft agent capabilities directly
