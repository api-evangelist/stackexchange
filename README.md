# Stack Exchange (stackexchange)
Stack Exchange is the network of Q&A communities founded by Joel Spolsky and Jeff Atwood and headlined by Stack Overflow, the largest community of software developers on the web. The Stack Exchange API v2.3 (api.stackexchange.com) is a single, read-mostly HTTP/JSON interface that spans 180+ Q&A sites — Stack Overflow, Server Fault, Super User, Ask Ubuntu, Stats, Math Overflow, and the long tail of topical communities — and exposes the entire Q&A graph (questions, answers, comments, users, tags, badges, reputation, revisions, notifications, inbox, suggested-edits, network sites) under a uniform method surface. Stack Exchange also operates Stack Overflow for Teams (private knowledge bases with its own v3 REST API) and ships an official Stack Overflow MCP server that grounds AI agents in community-verified content.

**URL:** [Visit APIs.json URL](https://api.stackexchange.com/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Q And A, Developer Community, Knowledge Graph, Stack Overflow, Stack Exchange, Reputation, Tags, Community, MCP, AI Grounding

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### Stack Exchange API v2.3
Public, read-mostly HTTP/JSON API spanning all 180+ Stack Exchange sites. All method families — questions, answers, comments, users, tags, badges, sites, search, /me, access-tokens, notifications, inbox, events, revisions, info, reputation, privileges, suggested-edits, posts — live under a single base URL with a uniform response wrapper (items, has_more, page, quota_max, quota_remaining, backoff). Read access requires no auth; writes (posting, voting, flagging, accepting) require OAuth 2.0 with the appropriate scopes (write_access, private_info, no_expiry).

**Human URL:** [https://api.stackexchange.com/docs](https://api.stackexchange.com/docs)

**Base URL:** `https://api.stackexchange.com/2.3`

#### Tags:

 - Stack Exchange, Public API, Q And A, Read-Mostly, OAuth 2.0

#### Properties

- [Documentation](https://api.stackexchange.com/docs)
- [OpenAPI](openapi/stackexchange-api-v2-3.yaml)
- [SignUp](https://stackapps.com/apps/oauth/register)
- [Authentication](https://api.stackexchange.com/docs/authentication)
- [TermsOfService](https://stackoverflow.com/legal/api-terms-of-use)
- [Throttling](https://api.stackexchange.com/docs/throttle)
- [Filters](https://api.stackexchange.com/docs/filters)
- [ChangeLog](https://api.stackexchange.com/docs/revisions)
- [SDK — .NET (StacMan)](https://github.com/StackExchange/StacMan)
- [NaftikoCapability](capabilities/stack-exchange-questions.yaml)
- [NaftikoCapability](capabilities/stack-exchange-answers.yaml)
- [NaftikoCapability](capabilities/stack-exchange-comments.yaml)
- [NaftikoCapability](capabilities/stack-exchange-users.yaml)
- [NaftikoCapability](capabilities/stack-exchange-me.yaml)
- [NaftikoCapability](capabilities/stack-exchange-tags.yaml)
- [NaftikoCapability](capabilities/stack-exchange-badges.yaml)
- [NaftikoCapability](capabilities/stack-exchange-sites.yaml)
- [NaftikoCapability](capabilities/stack-exchange-search.yaml)
- [NaftikoCapability](capabilities/stack-exchange-posts.yaml)
- [NaftikoCapability](capabilities/stack-exchange-revisions.yaml)
- [NaftikoCapability](capabilities/stack-exchange-suggested-edits.yaml)
- [NaftikoCapability](capabilities/stack-exchange-events.yaml)
- [NaftikoCapability](capabilities/stack-exchange-info.yaml)
- [NaftikoCapability](capabilities/stack-exchange-access-tokens.yaml)
- [NaftikoCapability](capabilities/stack-exchange-filters.yaml)

### Stack Overflow for Teams API v3
Newer REST API powering Stack Overflow for Teams (private/internal instances). Resource-oriented (questions, answers, articles, comments, tags, users, collections, communities) with full CRUD and bearer-token auth. This is the API the official TypeScript SDK and Terraform provider target; it is distinct from the public v2.3 API.

**Human URL:** [https://stackoverflowteams.help/en/articles/9085836-api-v3-overview](https://stackoverflowteams.help/en/articles/9085836-api-v3-overview)

**Base URL:** `https://api.stackoverflowteams.com/v3/teams/{team}/`

#### Tags:

 - Stack Overflow for Teams, Internal API, REST, Bearer Token

#### Properties

- [Documentation](https://stackoverflowteams.help/en/articles/9085836-api-v3-overview)
- [SDK — TypeScript SDK](https://www.npmjs.com/package/@stackoverflow/teams-sdk)
- [SDK — TypeScript SDK Source](https://github.com/StackExchange/StackOverflowSDK)
- [Tools — Terraform Provider](https://github.com/StackExchange/terraform-provider-stackoverflow)
- [Tools — Backstage Plugin](https://github.com/StackExchange/backstage-stackoverflow)
- [Tools — LangChain Integration](https://github.com/StackExchange/langchain-stack-overflow-for-teams)

## Common Properties

- [Website](https://stackexchange.com/)
- [Documentation](https://api.stackexchange.com/docs)
- [DeveloperPortal](https://stackapps.com/)
- [GitHubOrganization](https://github.com/StackExchange)
- [Blog](https://stackoverflow.blog/)
- [TermsOfService](https://stackoverflow.com/legal/api-terms-of-use)
- [PrivacyPolicy](https://stackoverflow.com/legal/privacy-policy)
- [StatusPage](https://stackstatus.tumblr.com/)
- [ApplicationRegistration](https://stackapps.com/apps/oauth/register)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [Tools — MCP Server (Stack Overflow)](https://github.com/StackExchange/Stack-MCP)
- [Tools — MCP Server Documentation](https://api.stackexchange.com/docs/mcp-server)
- [Tools — Stack Exchange Data Explorer](https://github.com/StackExchange/StackExchange.DataExplorer)
- [Tools — Stacks Design System](https://github.com/StackExchange/Stacks)
- [Plans](plans/stackexchange-plans-pricing.yml)
- [RateLimits](rate-limits/stackexchange-rate-limits.yml)
- [Rules](rules/stackexchange-spectral-rules.yml)
- [Vocabulary](vocabulary/stackexchange-vocabulary.yml)

## Features

| Name | Description |
|------|-------------|
| Network-Wide Q&A Graph | Single API surface spans 180+ communities. Use the `site` parameter (`stackoverflow`, `serverfault`, `superuser`, `askubuntu`, `stats`, `mathoverflow`, …) to switch context without changing endpoints. |
| Vectorized IDs | Most methods accept up to 100 semicolon-delimited IDs in a single request (e.g., `/questions/{ids}`, `/users/{ids}`, `/answers/{ids}`), making bulk fetch and join workloads cheap. |
| Filter System | Custom response filters let consumers project exactly the fields they need, dramatically reducing payload size. Filters are created once via `/filters/create` and reused. |
| Compressed JSON | All responses are gzip-compressed by default; the wire payload is roughly 30-50% the size of an unconditioned JSON body. |
| Quota and Backoff Discipline | Every response advertises `quota_max`, `quota_remaining`, and an optional `backoff` integer. Clients must honor the backoff before re-querying the same method or risk being throttled at 503 / banned. |
| OAuth 2.0 Write Access | Read is unauthenticated. Write methods (post answer, create comment, vote, flag, accept) require an OAuth 2.0 access token issued via explicit or implicit flows registered on stackapps.com. |
| /me Convenience Methods | Every `/users/{ids}/...` method has a `/me/...` equivalent that infers the user from the access token, simplifying agent code paths. |
| Site Discovery | `/sites` enumerates every Q&A community on the network with its `api_site_parameter`, audience, launch date, and styling — the canonical way to bootstrap a multi-site integration. |
| AI Grounding via MCP | The official Stack Overflow MCP server exposes search, retrieve, and ground tools so MCP-compatible clients (Claude Desktop, Cursor, VS Code) can reach community-verified answers without bespoke integration. |

## Use Cases

| Name | Description |
|------|-------------|
| AI Answer Grounding | Ground LLM responses in real Stack Overflow questions and answers — either directly via /search and /questions methods or through the official MCP server — to reduce hallucinations on technical topics. |
| Developer Reputation Scoring | Pull /users, /users/{ids}/reputation, badge counts, and tag scores to build developer reputation, expertise, and hiring-signal pipelines. |
| Community Analytics | Aggregate /questions, /tags, /tags/{tags}/info, and /sites data to track technology adoption, tag velocity, and community health across the network. |
| Personal Activity Dashboards | Use /me, /me/inbox, /me/notifications, /me/timeline, /me/answers, and /me/questions to build personal dashboards of a user's own activity, reputation, and unread events. |
| Tag Tracking and Triage | Watch /tags/{tags}/info, /questions?tagged=…, /search/advanced, and /questions/no-answers to triage incoming questions for OSS projects and vendor support teams. |
| Knowledge Base Mirroring | Periodically sweep /questions with a filter and a since-date to mirror Q&A into an internal knowledge base or RAG index, respecting the API quota and backoff. |
| Moderation Workbench | Combine /suggested-edits, /flags, /posts, and /revisions surfaces (with a moderator access token) to build moderation review queues. |
| Stack Overflow for Teams Integrations | Use the v3 Teams API plus the Terraform provider and Backstage plugin to provision questions, articles, and tags from CI/CD pipelines. |

## Integrations

| Name | Description |
|------|-------------|
| Claude Desktop / Cursor / VS Code via MCP | The Stack Overflow MCP server plugs directly into any MCP-compatible client, giving AI agents a typed search/retrieve interface to community content. |
| LangChain | Official LangChain integration for Stack Overflow for Teams enables retrieval and chat over private Teams content from LangChain pipelines. |
| Backstage | Backstage plugin (`backstage-stackoverflow`) surfaces Stack Overflow for Teams content inside Backstage developer portals. |
| Terraform | Terraform provider (`terraform-provider-stackoverflow`) manages questions, answers, and articles in Stack Overflow for Teams as code. |
| StacMan (.NET) | Long-standing .NET client for Stack Exchange API v2 (StackExchange/StacMan) covering the public v2.3 surface. |

## Solutions

| Name | Description |
|------|-------------|
| Public API v2.3 | Read-mostly, unauthenticated public access to the full Q&A graph across 180+ sites. Default integration path for developer tools, dashboards, community analytics, and AI grounding. |
| Stack Overflow for Teams API v3 | Private REST API for Stack Overflow for Teams customers, used by the TypeScript SDK, Terraform provider, Backstage plugin, and LangChain integration. |
| Stack Overflow MCP Server | Beta MCP server that lets MCP-compatible AI clients search, retrieve, and ground answers in Stack Overflow content with simple OAuth onboarding. |
| Stack Exchange Data Explorer | SQL-style query interface for the Stack Exchange data dumps, used for analytics workloads that exceed the API quota. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [stackexchange-api-v2-3.yaml](openapi/stackexchange-api-v2-3.yaml)

### JSON Schema

- [stackexchange-api-v2-3-access-token-schema.json](json-schema/stackexchange-api-v2-3-access-token-schema.json)
- [stackexchange-api-v2-3-answer-schema.json](json-schema/stackexchange-api-v2-3-answer-schema.json)
- [stackexchange-api-v2-3-badge-count-schema.json](json-schema/stackexchange-api-v2-3-badge-count-schema.json)
- [stackexchange-api-v2-3-badge-schema.json](json-schema/stackexchange-api-v2-3-badge-schema.json)
- [stackexchange-api-v2-3-comment-schema.json](json-schema/stackexchange-api-v2-3-comment-schema.json)
- [stackexchange-api-v2-3-event-schema.json](json-schema/stackexchange-api-v2-3-event-schema.json)
- [stackexchange-api-v2-3-filter-schema.json](json-schema/stackexchange-api-v2-3-filter-schema.json)
- [stackexchange-api-v2-3-inbox-item-schema.json](json-schema/stackexchange-api-v2-3-inbox-item-schema.json)
- [stackexchange-api-v2-3-info-schema.json](json-schema/stackexchange-api-v2-3-info-schema.json)
- [stackexchange-api-v2-3-notification-schema.json](json-schema/stackexchange-api-v2-3-notification-schema.json)
- [stackexchange-api-v2-3-post-schema.json](json-schema/stackexchange-api-v2-3-post-schema.json)
- [stackexchange-api-v2-3-privilege-item-schema.json](json-schema/stackexchange-api-v2-3-privilege-item-schema.json)
- [stackexchange-api-v2-3-question-schema.json](json-schema/stackexchange-api-v2-3-question-schema.json)
- [stackexchange-api-v2-3-reputation-change-schema.json](json-schema/stackexchange-api-v2-3-reputation-change-schema.json)
- [stackexchange-api-v2-3-revision-schema.json](json-schema/stackexchange-api-v2-3-revision-schema.json)
- [stackexchange-api-v2-3-shallow-user-schema.json](json-schema/stackexchange-api-v2-3-shallow-user-schema.json)
- [stackexchange-api-v2-3-site-schema.json](json-schema/stackexchange-api-v2-3-site-schema.json)
- [stackexchange-api-v2-3-suggested-edit-schema.json](json-schema/stackexchange-api-v2-3-suggested-edit-schema.json)
- [stackexchange-api-v2-3-tag-schema.json](json-schema/stackexchange-api-v2-3-tag-schema.json)
- [stackexchange-api-v2-3-tag-score-schema.json](json-schema/stackexchange-api-v2-3-tag-score-schema.json)
- [stackexchange-api-v2-3-tag-synonym-schema.json](json-schema/stackexchange-api-v2-3-tag-synonym-schema.json)
- [stackexchange-api-v2-3-user-schema.json](json-schema/stackexchange-api-v2-3-user-schema.json)

### JSON Structure

- [stackexchange-api-v2-3-access-token-structure.json](json-structure/stackexchange-api-v2-3-access-token-structure.json)
- [stackexchange-api-v2-3-answer-structure.json](json-structure/stackexchange-api-v2-3-answer-structure.json)
- [stackexchange-api-v2-3-badge-count-structure.json](json-structure/stackexchange-api-v2-3-badge-count-structure.json)
- [stackexchange-api-v2-3-badge-structure.json](json-structure/stackexchange-api-v2-3-badge-structure.json)
- [stackexchange-api-v2-3-comment-structure.json](json-structure/stackexchange-api-v2-3-comment-structure.json)
- [stackexchange-api-v2-3-event-structure.json](json-structure/stackexchange-api-v2-3-event-structure.json)
- [stackexchange-api-v2-3-filter-structure.json](json-structure/stackexchange-api-v2-3-filter-structure.json)
- [stackexchange-api-v2-3-inbox-item-structure.json](json-structure/stackexchange-api-v2-3-inbox-item-structure.json)
- [stackexchange-api-v2-3-info-structure.json](json-structure/stackexchange-api-v2-3-info-structure.json)
- [stackexchange-api-v2-3-notification-structure.json](json-structure/stackexchange-api-v2-3-notification-structure.json)
- [stackexchange-api-v2-3-post-structure.json](json-structure/stackexchange-api-v2-3-post-structure.json)
- [stackexchange-api-v2-3-privilege-item-structure.json](json-structure/stackexchange-api-v2-3-privilege-item-structure.json)
- [stackexchange-api-v2-3-question-structure.json](json-structure/stackexchange-api-v2-3-question-structure.json)
- [stackexchange-api-v2-3-reputation-change-structure.json](json-structure/stackexchange-api-v2-3-reputation-change-structure.json)
- [stackexchange-api-v2-3-revision-structure.json](json-structure/stackexchange-api-v2-3-revision-structure.json)
- [stackexchange-api-v2-3-shallow-user-structure.json](json-structure/stackexchange-api-v2-3-shallow-user-structure.json)
- [stackexchange-api-v2-3-site-structure.json](json-structure/stackexchange-api-v2-3-site-structure.json)
- [stackexchange-api-v2-3-suggested-edit-structure.json](json-structure/stackexchange-api-v2-3-suggested-edit-structure.json)
- [stackexchange-api-v2-3-tag-score-structure.json](json-structure/stackexchange-api-v2-3-tag-score-structure.json)
- [stackexchange-api-v2-3-tag-structure.json](json-structure/stackexchange-api-v2-3-tag-structure.json)
- [stackexchange-api-v2-3-tag-synonym-structure.json](json-structure/stackexchange-api-v2-3-tag-synonym-structure.json)
- [stackexchange-api-v2-3-user-structure.json](json-structure/stackexchange-api-v2-3-user-structure.json)

### JSON-LD

- [stackexchange-api-v2-3-context.jsonld](json-ld/stackexchange-api-v2-3-context.jsonld)

### Examples

- [stackexchange-api-v2-3-access-token-example.json](examples/stackexchange-api-v2-3-access-token-example.json)
- [stackexchange-api-v2-3-answer-example.json](examples/stackexchange-api-v2-3-answer-example.json)
- [stackexchange-api-v2-3-badge-count-example.json](examples/stackexchange-api-v2-3-badge-count-example.json)
- [stackexchange-api-v2-3-badge-example.json](examples/stackexchange-api-v2-3-badge-example.json)
- [stackexchange-api-v2-3-comment-example.json](examples/stackexchange-api-v2-3-comment-example.json)
- [stackexchange-api-v2-3-event-example.json](examples/stackexchange-api-v2-3-event-example.json)
- [stackexchange-api-v2-3-filter-example.json](examples/stackexchange-api-v2-3-filter-example.json)
- [stackexchange-api-v2-3-inbox-item-example.json](examples/stackexchange-api-v2-3-inbox-item-example.json)
- [stackexchange-api-v2-3-info-example.json](examples/stackexchange-api-v2-3-info-example.json)
- [stackexchange-api-v2-3-notification-example.json](examples/stackexchange-api-v2-3-notification-example.json)
- [stackexchange-api-v2-3-post-example.json](examples/stackexchange-api-v2-3-post-example.json)
- [stackexchange-api-v2-3-privilege-item-example.json](examples/stackexchange-api-v2-3-privilege-item-example.json)
- [stackexchange-api-v2-3-question-example.json](examples/stackexchange-api-v2-3-question-example.json)
- [stackexchange-api-v2-3-reputation-change-example.json](examples/stackexchange-api-v2-3-reputation-change-example.json)
- [stackexchange-api-v2-3-revision-example.json](examples/stackexchange-api-v2-3-revision-example.json)
- [stackexchange-api-v2-3-shallow-user-example.json](examples/stackexchange-api-v2-3-shallow-user-example.json)
- [stackexchange-api-v2-3-site-example.json](examples/stackexchange-api-v2-3-site-example.json)
- [stackexchange-api-v2-3-suggested-edit-example.json](examples/stackexchange-api-v2-3-suggested-edit-example.json)
- [stackexchange-api-v2-3-tag-example.json](examples/stackexchange-api-v2-3-tag-example.json)
- [stackexchange-api-v2-3-tag-score-example.json](examples/stackexchange-api-v2-3-tag-score-example.json)
- [stackexchange-api-v2-3-tag-synonym-example.json](examples/stackexchange-api-v2-3-tag-synonym-example.json)
- [stackexchange-api-v2-3-user-example.json](examples/stackexchange-api-v2-3-user-example.json)

## Capabilities

Self-contained Naftiko capabilities — one file per business surface (OpenAPI tag), each with consumes + REST + MCP exposers inlined.

| Capability | Tools | File |
|------------|-------|------|
| Stack Exchange API v2.3 — Access Tokens | 3 | [stack-exchange-access-tokens.yaml](capabilities/stack-exchange-access-tokens.yaml) |
| Stack Exchange API v2.3 — Answers | 4 | [stack-exchange-answers.yaml](capabilities/stack-exchange-answers.yaml) |
| Stack Exchange API v2.3 — Badges | 5 | [stack-exchange-badges.yaml](capabilities/stack-exchange-badges.yaml) |
| Stack Exchange API v2.3 — Comments | 2 | [stack-exchange-comments.yaml](capabilities/stack-exchange-comments.yaml) |
| Stack Exchange API v2.3 — Events | 1 | [stack-exchange-events.yaml](capabilities/stack-exchange-events.yaml) |
| Stack Exchange API v2.3 — Filters | 2 | [stack-exchange-filters.yaml](capabilities/stack-exchange-filters.yaml) |
| Stack Exchange API v2.3 — Info | 1 | [stack-exchange-info.yaml](capabilities/stack-exchange-info.yaml) |
| Stack Exchange API v2.3 — Me | 12 | [stack-exchange-me.yaml](capabilities/stack-exchange-me.yaml) |
| Stack Exchange API v2.3 — Posts | 5 | [stack-exchange-posts.yaml](capabilities/stack-exchange-posts.yaml) |
| Stack Exchange API v2.3 — Questions | 9 | [stack-exchange-questions.yaml](capabilities/stack-exchange-questions.yaml) |
| Stack Exchange API v2.3 — Revisions | 1 | [stack-exchange-revisions.yaml](capabilities/stack-exchange-revisions.yaml) |
| Stack Exchange API v2.3 — Search | 4 | [stack-exchange-search.yaml](capabilities/stack-exchange-search.yaml) |
| Stack Exchange API v2.3 — Sites | 1 | [stack-exchange-sites.yaml](capabilities/stack-exchange-sites.yaml) |
| Stack Exchange API v2.3 — Suggested Edits | 2 | [stack-exchange-suggested-edits.yaml](capabilities/stack-exchange-suggested-edits.yaml) |
| Stack Exchange API v2.3 — Tags | 7 | [stack-exchange-tags.yaml](capabilities/stack-exchange-tags.yaml) |
| Stack Exchange API v2.3 — Users | 11 | [stack-exchange-users.yaml](capabilities/stack-exchange-users.yaml) |

## Vocabulary

- [Stack Exchange Vocabulary](vocabulary/stackexchange-vocabulary.yml) — 16 resources, 8 actions, 16 workflows, 11 personas

## Rules

- [Stack Exchange Spectral Ruleset](rules/stackexchange-spectral-rules.yml) — 44 rules enforcing Stack Exchange API conventions

## Plans

- [Stack Exchange Plans & Pricing](plans/stackexchange-plans-pricing.yml) — 3 plans (API Commons Plans 0.1)

## Rate Limits

- [Stack Exchange Rate Limits](rate-limits/stackexchange-rate-limits.yml) — 6 limits, 7 policies (API Commons Rate Limits 0.1)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
