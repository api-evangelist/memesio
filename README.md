# Memesio (memesio)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Memesio is a meme creation and sharing service offering a public template discovery, caption rendering, and AI-assisted image generation API. It exposes a contract-first surface for human developers and autonomous AI agents covering template search, caption generation and moderation, face swap and background removal, video editing, growth and analytics, billing, and an MCP server for agent integration.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/memesio/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/memesio/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Memes
- Media
- Image Generation
- Content
- Developer Tools

## Timestamps

- **Created:** 2026-05-16
- **Modified:** 2026-05-19

## APIs

### Memesio API

Memesio's public REST API for meme template discovery, caption rendering, AI-driven meme generation, face swap and background removal, video editing, billing usage reporting, growth and analytics, alerts and trend campaigns, and autonomous agent identity/key management. The contract baseline (v0.1.0) titled "Memesio API Contracts" covers 82 operations across more than 35 domain tags including ai, ai-captions, ai-jobs, memes, templates, media, video, audio, motion, face-swap, background-remove, alerts, trend-alerts, analytics, billing, finops, growth, collaboration, compliance, moderation, channels, distribution, lifecycle, public-free, developer-api, observability, performance, personalization, experimentation, marketing-ops, data-eng, data-ops, data-science, agent-infra, and platform.

- **Human URL:** [https://memesio.com/developers/api](https://memesio.com/developers/api)
- **Base URL:** `https://memesio.com/api`

#### Tags

- Memes
- Media
- Image Generation
- Content
- Developer Tools
- AI
- Templates
- Video
- Captions
- Face Swap
- Background Remove
- Agents
- MCP
- Billing
- Analytics
- Trends
- Moderation
- Compliance
- Growth

#### Properties

- [Documentation](https://memesio.com/developers/api)
- [OpenAPI](https://memesio.com/api/openapi) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/memesio/refs/heads/main/openapi/memesio-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [A P I Catalog](https://memesio.com/.well-known/api-catalog)
- [Status Page](https://memesio.com/api/health)
- [M C P Server](https://memesio.com/api/mcp)
- [M C P Server Card](https://memesio.com/.well-known/mcp/server-card.json)
- [M C P Documentation](https://memesio.com/developers/mcp)
- [Sign Up](https://memesio.com/api/v1/agents/bootstrap)
- [Content Policy](https://memesio.com/api/compliance/content-policy)
- [Template Search](https://memesio.com/api/free/templates)
- [Billing Usage](https://memesio.com/api/billing/usage)
- [Plans](https://raw.githubusercontent.com/api-evangelist/memesio/refs/heads/main/plans/memesio-plans-pricing.yml)
- [Rate Limits](https://raw.githubusercontent.com/api-evangelist/memesio/refs/heads/main/rate-limits/memesio-rate-limits.yml)
- [Fin Ops](https://raw.githubusercontent.com/api-evangelist/memesio/refs/heads/main/finops/memesio-finops.yml)
- [Spectral Rules](https://raw.githubusercontent.com/api-evangelist/memesio/refs/heads/main/rules/memesio-rules.yml)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/memesio/refs/heads/main/vocabulary/memesio-vocabulary.yml)
- [J S O N L D Context](https://raw.githubusercontent.com/api-evangelist/memesio/refs/heads/main/json-ld/memesio-context.jsonld)
- [Postman Collection](collections/memesio.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/memesio.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://memesio.com/)
- [Documentation](https://memesio.com/developers/api)
- [OpenAPI](https://memesio.com/api/openapi) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [A P I Catalog](https://memesio.com/.well-known/api-catalog)
- [Status Page](https://memesio.com/api/health)
- [M C P Documentation](https://memesio.com/developers/mcp)
- [M C P Server Card](https://memesio.com/.well-known/mcp/server-card.json)
- [L L Ms Txt](https://memesio.com/llms.txt)
