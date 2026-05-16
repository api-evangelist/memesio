# Memesio (memesio)

Memesio is a meme creation and sharing service offering a public template
discovery, caption rendering, and AI-assisted image generation API. The
service exposes a contract-first surface for human developers and autonomous
AI agents covering template search, caption generation and moderation, face
swap and background removal, video editing, growth and analytics, billing,
and an MCP server for agent integration.

- **Source:** https://memesio.com/
- **Documentation:** https://memesio.com/developers/api
- **OpenAPI:** https://memesio.com/api/openapi
- **API Catalog (RFC 9727):** https://memesio.com/.well-known/api-catalog
- **MCP Server Card:** https://memesio.com/.well-known/mcp/server-card.json
- **MCP Documentation:** https://memesio.com/developers/mcp
- **Status / Health:** https://memesio.com/api/health
- **Agent Signup (Bootstrap):** `POST https://memesio.com/api/v1/agents/bootstrap`
- **api-search issue:** [#28](https://github.com/api-search/network/issues/28)

## API Surface

The real OpenAPI 3.1 contract ("Memesio API Contracts v0.1.0") describes
**82 paths / 111 operations / 23 component schemas** across more than 35
domain tags including: `ai`, `ai-captions`, `ai-jobs`, `ai-providers`,
`memes`, `templates`, `media`, `video`, `motion`, `audio`, `face-swap`,
`background-remove`, `alerts`, `trend-alerts`, `analytics`, `billing`,
`finops`, `growth`, `collaboration`, `compliance`, `moderation`, `channels`,
`distribution`, `lifecycle`, `public-free`, `developer-api`, `observability`,
`performance`, `personalization`, `experimentation`, `marketing-ops`,
`data-eng`, `data-ops`, `data-science`, `agent-infra`, and `platform`.

The service also publishes a sibling MCP server
(`https://memesio.com/api/mcp`, streamable-http) exposing seven tools:
`create_agent_account`, `search_templates`, `get_template_ideas`,
`caption_template`, `caption_upload`, `generate_meme`, `get_ai_quota`.

## Authentication

| Caller | Auth | Header |
|---|---|---|
| Anonymous | none | (template discovery + free caption with watermark) |
| Developer | API key | `x-agent-api-key` |
| Agent | API key | `x-agent-api-key` (bootstrapped via `/api/v1/agents/bootstrap`) |
| Editor | session | first-party only |

## Plans, Rate Limits, FinOps

Memesio uses a **quota-based** plan model; there is no public price sheet
at `https://memesio.com/pricing` (404). See:

- [plans/memesio-plans-pricing.yml](plans/memesio-plans-pricing.yml) — Anonymous, Developer, Agent, Premium (custom).
- [rate-limits/memesio-rate-limits.yml](rate-limits/memesio-rate-limits.yml) — AI quota 3/day baseline, variants/request 5 max, agent default 1 variant, template pageSize 50 max.
- [finops/memesio-finops.yml](finops/memesio-finops.yml) — `/api/billing/usage` returns 30-day metered usage with estimated USD by event and AI provider/capability.

All three carry `reconciled: false` because the underlying monetary rates
and per-key rate-limit numerics are not publicly disclosed by Memesio.

## Generated Artifacts

| Folder | Contents |
|---|---|
| [openapi/](openapi/) | Memesio OpenAPI 3.1 contract (YAML) |
| [rules/](rules/) | Spectral ruleset enforcing Memesio path, tag, and quota conventions |
| [capabilities/](capabilities/) | Naftiko workflows: meme creation, AI captions, agent identity, video production, trends & growth + shared per-API definition |
| [json-schema/](json-schema/) | 23 JSON Schema 2020-12 files (one per OpenAPI component) |
| [json-structure/](json-structure/) | 23 JSON Structure equivalents |
| [json-ld/](json-ld/) | JSON-LD context aligning Memesio vocabulary with schema.org |
| [examples/](examples/) | 111 generated operation example pairs + curated real-data examples (template search, caption template, AI generate, agent bootstrap, billing usage, content policy) |
| [vocabulary/](vocabulary/) | Memesio operational vocabulary (concepts, services, tools, standards, tags) |
| [plans/](plans/) | API Commons Plans 0.1 |
| [rate-limits/](rate-limits/) | API Commons Rate Limits 0.1 |
| [finops/](finops/) | FinOps Framework / FOCUS 1.0 mapping |

## Notes

- No public GitHub org or user repositories: `https://github.com/memesio` exists as a user with **0 public repos**; there is no `github.com/memesio` org.
- Memesio's primary public discovery surface is `https://memesio.com/.well-known/api-catalog` (RFC 9727 linkset).
