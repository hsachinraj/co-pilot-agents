# Source Guidelines

Best practices for collecting, validating, and citing competitive intelligence.

## Official Sources (Priority Order)

1. **Vendor documentation**  
   - Product docs, API references, feature pages
   - Example: `docs.anthropic.com`, `docs.aws.amazon.com/bedrock`

2. **Official blogs & announcements**  
   - Vendor announcements, release notes, blog posts
   - Example: OpenAI announcements, AWS What's New

3. **Keynote/conference talks**  
   - Official vendor presentations at conferences (I/O, AWS re:Invent, etc.)
   - Look for timestamp + video link

4. **Official social media** (if no docs exist)  
   - Twitter/X, LinkedIn posts from official accounts
   - Include post date + screenshot if link changes

## Secondary Sources (Use Only to Fill Gaps)

- **Trusted tech media**  
  - VentureBeat, The Verge, InfoQ, TechCrunch
  - Mark as `[media]` in your citation
  - Prefer if article links to official announcement

- **Developer forums & GitHub**  
  - GitHub releases, community forums, Discord
  - Use for "feature is available" confirmation, not feature claims

- **Third-party benchmarks**  
  - Use sparingly; always verify underlying data
  - Mark as `[3rd-party]` or `[benchmark]`

## Validation Checklist

Before including a claim:

- [ ] **Is there an official source?** (If yes, use it; don't cite media)
- [ ] **Is the claim timestamped?** (What date was it announced/released?)
- [ ] **Is the status clear?** (GA / Preview / Roadmap / Deprecated?)
- [ ] **Is it specific?** (Not vague like "improved performance")
- [ ] **Can I link directly?** (Reader should find proof in 10 seconds)
- [ ] **Is it still accurate?** (Vendor product pages change; confirm freshness)

## Citation Format

Use this consistent format across all competitive scans:

```markdown
[Capability]: [Status] ([Release Date]) – [Vendor] [Citation Format]
```

### Examples

**Official Source:**
```
Parallel tool calls: GA (2026-Q1) – OpenAI
[Blog post](https://openai.com/blog/function-calling-improvements)
[Official Docs](https://platform.openai.com/docs/guides/function-calling)
```

**Secondary Source:**
```
Long-context retrieval: Preview (2026-Q2) – AWS Bedrock
[AWS What's New](https://aws.amazon.com/about-aws/whats-new/bedrock)
[Media coverage](https://venturebeat.com/article-link)
```

**Roadmap Item:**
```
HIPAA compliance: Roadmap (2026-Q3) – Anthropic
[Roadmap page](https://www.anthropic.com/roadmap)
```

## Conflict Resolution

If sources disagree on capability status:

```markdown
Tool result streaming: **Status disputed**
- OpenAI: GA (2026-Q2) [official docs](link)
- AWS: Preview (2026-Q1) [media report](link)
→ **Action**: Verify with official docs; if unclear, report both versions
```

Do NOT pick a source and ignore the other. Flag it so readers know there's ambiguity.

## Freshness Guidelines

- **Check at least weekly** if tracking real-time updates
- **Note the check date** in your document: `Last checked: 2026-06-22`
- **Archive old versions** if you publish quarterly scans
- **Use "as of [date]"** when citing capability status that may have changed

## Template for Citation Section

Include this at the end of your competitive scan:

```markdown
## Sources & Freshness

Last scanned: **[Date]**

### Official Channels Checked
- ✅ OpenAI docs + blog
- ✅ AWS Bedrock what's new
- ✅ Google Vertex AI release notes
- ✅ Anthropic website + roadmap

### Secondary Sources
- VentureBeat (filtered by AI agent relevance)
- TechCrunch (announcements + funding)

### Known Gaps
- [Item not yet released / under NDA]
- [Vendor communication unclear on timing]
```

---

**Remember**: Your credibility depends on sourcing. When in doubt, cite multiple sources or say "unconfirmed."
