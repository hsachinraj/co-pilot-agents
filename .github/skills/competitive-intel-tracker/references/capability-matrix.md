# Capability Matrix Template

Use this template to standardize competitive capability comparisons across vendors.

## How to Use
1. Copy this template into your intelligence document
2. Fill in each cell with: **Status** (GA/Preview/Roadmap/Absent) + **Date** + **Source Link**
3. Update quarterly to track evolution

## Template

| Capability | OpenAI | AWS Bedrock | Google Vertex AI | Anthropic |
|---|---|---|---|---|
| **Orchestration** | | | | |
| Multi-step workflows | GA (2026-Q2) [link](https://openai.com/docs) | Preview (2026-Q1) [link](https://aws.amazon.com) | GA (2025-Q4) [link](https://cloud.google.com) | GA (2026-Q1) [link](https://anthropic.com) |
| Branching & conditionals | GA | GA | GA | Preview |
| Loop & retry logic | GA | GA | GA | GA |
| State persistence | GA | Preview | GA | Limited |
| **Tool Use** | | | | |
| Function calling | GA | GA | GA | GA |
| Parallel tool calls | GA | Preview | GA | GA |
| Tool result streaming | Preview | Roadmap | GA | GA |
| Dynamic tool discovery | GA | Limited | Preview | GA |
| **Memory & Context** | | | | |
| Multi-turn conversation | GA | GA | GA | GA |
| Long-context windows (100K+) | GA | GA | GA | GA |
| Structured state storage | Limited | GA | Preview | GA |
| Semantic caching | Preview (2026-Q2) | GA | GA | Roadmap |
| **Evaluation & Observability** | | | | |
| Built-in eval framework | GA | Limited | GA | Limited |
| Trace collection | GA | GA | GA | Limited |
| Structured tracing | GA | GA | Preview | Coming |
| Custom scorer support | GA | Limited | GA | GA |
| **Deployment & Runtime** | | | | |
| Serverless option | Yes (API) | Yes (Bedrock) | Yes (Vertex) | Yes (API) |
| Self-hosted option | Limited | Yes (On-Premises) | Yes (Duet) | No |
| Container runtime | No | Via Lambda | Yes | No |
| Autoscaling | Managed | Managed | Managed | Managed |
| **Security & Governance** | | | | |
| SOC 2 Type II | Yes | Yes | Yes | Yes |
| HIPAA compliance | Yes | Yes | Yes | Coming |
| Audit logging | GA | GA | GA | Limited |
| RBAC | Basic | Advanced | Advanced | Basic |
| **Pricing Model** | | | | |
| Usage-based | Yes | Yes | Yes | Yes |
| Per-message quota | Yes | Yes | Yes | No |
| Pricing transparency | Moderate | Good | Good | Good |
| Volume discounts | Via support | Yes | Yes | Via support |

## Notes

- **GA**: Generally Available (production-ready)
- **Preview**: Early/beta access (may have limitations, pricing TBD)
- **Roadmap**: Announced but not yet available
- **Absent**: Not offered
- **Limited**: Offered but with significant constraints (fewer options, restricted use cases)

**Last Updated**: [Date]  
**Sources**: [List official sources checked]
