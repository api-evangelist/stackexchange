# Stack Exchange

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

Stack Exchange is the network of Q&A communities founded by Joel Spolsky and Jeff Atwood and headlined by Stack Overflow, the largest community of software developers on the web. The Stack Exchange API v2.3 (api.stackexchange.com) is a single, read-mostly HTTP/JSON interface that spans 180+ Q&A sites — Stack Overflow, Server Fault, Super User, Ask Ubuntu, Stats, Math Overflow, and the long tail of topical communities — and exposes the entire Q&A graph (questions, answers, comments, users, tags, badges, reputation, revisions, notifications, inbox, suggested-edits, network sites) under a uniform method surface. Stack Exchange also operates Stack Overflow for Teams (private knowledge bases with its own v3 REST API) and ships an official Stack Overflow MCP server that grounds AI agents in community-verified content.

**Areas:** Q&A · Developer Community · Knowledge Graph · Stack Overflow · Stack Exchange · Reputation · Tags · Community · MCP · AI Grounding

## Stack Exchange on APIs.io

Everything profiled for Stack Exchange is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/stackexchange/](https://apis.io/providers/stackexchange/)** — or go straight to one of the APIs or properties below.

### APIs (17)

- [Stack Overflow for Teams API v3](https://apis.io/apis/stackexchange/stack-overflow-for-teams-api-v3/) — Newer REST API powering Stack Overflow for Teams (private/internal instances). Resource-oriented (questions, answers, articles, comments, tags, users,…
- [Stack Exchange Access Tokens API](https://apis.io/apis/stackexchange/stackexchange-access-tokens-api/) — OAuth access token introspection and invalidation.
- [Stack Exchange Answers API](https://apis.io/apis/stackexchange/stackexchange-answers-api/) — Answer objects — list, fetch by id, and per-question answers.
- [Stack Exchange Badges API](https://apis.io/apis/stackexchange/stackexchange-badges-api/) — Badges defined on a site — by id, name, type, and recipients.
- [Stack Exchange Comments API](https://apis.io/apis/stackexchange/stackexchange-comments-api/) — Comments attached to questions and answers across the network.
- [Stack Exchange Events API](https://apis.io/apis/stackexchange/stackexchange-events-api/) — Recent network events (1.5 minute live window) for the authenticated user.
- [Stack Exchange Filters API](https://apis.io/apis/stackexchange/stackexchange-filters-api/) — Custom response filter creation and inspection.
- [Stack Exchange Info API](https://apis.io/apis/stackexchange/stackexchange-info-api/) — Site-wide statistics, totals, and metadata.
- [Stack Exchange Me API](https://apis.io/apis/stackexchange/stackexchange-me-api/) — Convenience surfaces that infer the user from the OAuth access token.
- [Stack Exchange Posts API](https://apis.io/apis/stackexchange/stackexchange-posts-api/) — Generic post surfaces covering both questions and answers as `post` objects.
- [Stack Exchange Questions API](https://apis.io/apis/stackexchange/stackexchange-questions-api/) — Question objects across the network — list, fetch, related, linked, search-equivalents.
- [Stack Exchange Revisions API](https://apis.io/apis/stackexchange/stackexchange-revisions-api/) — Revision history for posts.
- [Stack Exchange Search API](https://apis.io/apis/stackexchange/stackexchange-search-api/) — Question search — basic title-match, full-text excerpts, and advanced.
- [Stack Exchange Sites API](https://apis.io/apis/stackexchange/stackexchange-sites-api/) — Enumeration and metadata for the 180+ Stack Exchange Q&A sites.
- [Stack Exchange Suggested Edits API](https://apis.io/apis/stackexchange/stackexchange-suggested-edits-api/) — Pending edits proposed by users awaiting review.
- [Stack Exchange Tags API](https://apis.io/apis/stackexchange/stackexchange-tags-api/) — Tag catalog, synonyms, wikis, top askers/answerers, and related tags.
- [Stack Exchange Users API](https://apis.io/apis/stackexchange/stackexchange-users-api/) — Site users, their reputation, badges, tags, top posts, timeline, and write surfaces.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Stackexchange Agentic Access](https://apis.io/agentic-access/stackexchange/stackexchange-agentic-access/)

#### JSON Schema (23)

The data models the API reads and writes.

- [AccessToken](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-access-token/)
- [Answer](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-answer/)
- [Badge](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-badge/)
- [BadgeCount](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-badge-count/)
- [Comment](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-comment/)
- [Event](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-event/)
- [Filter](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-filter/)
- [InboxItem](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-inbox-item/)
- [Info](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-info/)
- [Notification](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-notification/)
- [Post](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-post/)
- [PrivilegeItem](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-privilege-item/)
- [Question](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-question/)
- [ReputationChange](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-reputation-change/)
- [Revision](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-revision/)
- [ShallowUser](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-shallow-user/)
- [Site](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-site/)
- [SuggestedEdit](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-suggested-edit/)
- [Tag](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-tag/)
- [TagScore](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-tag-score/)
- [TagSynonym](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-tag-synonym/)
- [User](https://apis.io/schemas/stackexchange/stackexchange-api-v2-3-user/)
- [Stack Exchange Question](https://apis.io/schemas/stackexchange/stackexchange-question/)

#### JSON Structure (22)

Data models expressed in JSON Structure.

- [Stackexchange Api V2 3 Access Token Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-access-token-structure/)
- [Stackexchange Api V2 3 Answer Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-answer-structure/)
- [Stackexchange Api V2 3 Badge Count Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-badge-count-structure/)
- [Stackexchange Api V2 3 Badge Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-badge-structure/)
- [Stackexchange Api V2 3 Comment Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-comment-structure/)
- [Stackexchange Api V2 3 Event Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-event-structure/)
- [Stackexchange Api V2 3 Filter Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-filter-structure/)
- [Stackexchange Api V2 3 Inbox Item Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-inbox-item-structure/)
- [Stackexchange Api V2 3 Info Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-info-structure/)
- [Stackexchange Api V2 3 Notification Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-notification-structure/)
- [Stackexchange Api V2 3 Post Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-post-structure/)
- [Stackexchange Api V2 3 Privilege Item Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-privilege-item-structure/)
- [Stackexchange Api V2 3 Question Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-question-structure/)
- [Stackexchange Api V2 3 Reputation Change Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-reputation-change-structure/)
- [Stackexchange Api V2 3 Revision Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-revision-structure/)
- [Stackexchange Api V2 3 Shallow User Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-shallow-user-structure/)
- [Stackexchange Api V2 3 Site Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-site-structure/)
- [Stackexchange Api V2 3 Suggested Edit Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-suggested-edit-structure/)
- [Stackexchange Api V2 3 Tag Score Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-tag-score-structure/)
- [Stackexchange Api V2 3 Tag Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-tag-structure/)
- [Stackexchange Api V2 3 Tag Synonym Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-tag-synonym-structure/)
- [Stackexchange Api V2 3 User Structure](https://apis.io/json-structure/stackexchange/stackexchange-api-v2-3-user-structure/)

#### JSON-LD (2)

Linked-data contexts for the provider's vocabulary.

- [Stackexchange Api V2 3 Context](https://apis.io/jsonld/stackexchange/stackexchange-api-v2-3-context/)
- [Stackexchange Context](https://apis.io/jsonld/stackexchange/stackexchange-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Stackexchange Vocabulary](https://apis.io/vocabularies/stackexchange/stackexchange-vocabulary/)

#### Examples (22)

Example requests and responses.

- [Stackexchange Api V2 3 Access Token Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-access-token-example/)
- [Stackexchange Api V2 3 Answer Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-answer-example/)
- [Stackexchange Api V2 3 Badge Count Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-badge-count-example/)
- [Stackexchange Api V2 3 Badge Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-badge-example/)
- [Stackexchange Api V2 3 Comment Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-comment-example/)
- [Stackexchange Api V2 3 Event Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-event-example/)
- [Stackexchange Api V2 3 Filter Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-filter-example/)
- [Stackexchange Api V2 3 Inbox Item Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-inbox-item-example/)
- [Stackexchange Api V2 3 Info Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-info-example/)
- [Stackexchange Api V2 3 Notification Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-notification-example/)
- [Stackexchange Api V2 3 Post Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-post-example/)
- [Stackexchange Api V2 3 Privilege Item Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-privilege-item-example/)
- [Stackexchange Api V2 3 Question Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-question-example/)
- [Stackexchange Api V2 3 Reputation Change Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-reputation-change-example/)
- [Stackexchange Api V2 3 Revision Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-revision-example/)
- [Stackexchange Api V2 3 Shallow User Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-shallow-user-example/)
- [Stackexchange Api V2 3 Site Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-site-example/)
- [Stackexchange Api V2 3 Suggested Edit Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-suggested-edit-example/)
- [Stackexchange Api V2 3 Tag Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-tag-example/)
- [Stackexchange Api V2 3 Tag Score Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-tag-score-example/)
- [Stackexchange Api V2 3 Tag Synonym Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-tag-synonym-example/)
- [Stackexchange Api V2 3 User Example](https://apis.io/examples/stackexchange/stackexchange-api-v2-3-user-example/)

#### Collections (32)

Postman and Open Collection request collections.

- [Stack Exchange Access Tokens API](https://apis.io/collections/stackexchange/open-stackexchange-access-tokens-api/)
- [Stack Exchange Access Tokens Answers API](https://apis.io/collections/stackexchange/open-stackexchange-answers-api/)
- [Stack Exchange Access Tokens Badges API](https://apis.io/collections/stackexchange/open-stackexchange-badges-api/)
- [Stack Exchange Access Tokens Comments API](https://apis.io/collections/stackexchange/open-stackexchange-comments-api/)
- [Stack Exchange Access Tokens Events API](https://apis.io/collections/stackexchange/open-stackexchange-events-api/)
- [Stack Exchange Access Tokens Filters API](https://apis.io/collections/stackexchange/open-stackexchange-filters-api/)
- [Stack Exchange Access Tokens Info API](https://apis.io/collections/stackexchange/open-stackexchange-info-api/)
- [Stack Exchange Access Tokens Me API](https://apis.io/collections/stackexchange/open-stackexchange-me-api/)
- [Stack Exchange Access Tokens Posts API](https://apis.io/collections/stackexchange/open-stackexchange-posts-api/)
- [Stack Exchange Access Tokens Questions API](https://apis.io/collections/stackexchange/open-stackexchange-questions-api/)
- [Stack Exchange Access Tokens Revisions API](https://apis.io/collections/stackexchange/open-stackexchange-revisions-api/)
- [Stack Exchange Access Tokens Search API](https://apis.io/collections/stackexchange/open-stackexchange-search-api/)
- [Stack Exchange Access Tokens Sites API](https://apis.io/collections/stackexchange/open-stackexchange-sites-api/)
- [Stack Exchange Access Tokens Suggested Edits API](https://apis.io/collections/stackexchange/open-stackexchange-suggested-edits-api/)
- [Stack Exchange Access Tokens Tags API](https://apis.io/collections/stackexchange/open-stackexchange-tags-api/)
- [Stack Exchange Access Tokens Users API](https://apis.io/collections/stackexchange/open-stackexchange-users-api/)
- [Stack Exchange Access Tokens API](https://apis.io/collections/stackexchange/postman-stackexchange-access-tokens-api/)
- [Stack Exchange Access Tokens Answers API](https://apis.io/collections/stackexchange/postman-stackexchange-answers-api/)
- [Stack Exchange Access Tokens Badges API](https://apis.io/collections/stackexchange/postman-stackexchange-badges-api/)
- [Stack Exchange Access Tokens Comments API](https://apis.io/collections/stackexchange/postman-stackexchange-comments-api/)
- [Stack Exchange Access Tokens Events API](https://apis.io/collections/stackexchange/postman-stackexchange-events-api/)
- [Stack Exchange Access Tokens Filters API](https://apis.io/collections/stackexchange/postman-stackexchange-filters-api/)
- [Stack Exchange Access Tokens Info API](https://apis.io/collections/stackexchange/postman-stackexchange-info-api/)
- [Stack Exchange Access Tokens Me API](https://apis.io/collections/stackexchange/postman-stackexchange-me-api/)
- [Stack Exchange Access Tokens Posts API](https://apis.io/collections/stackexchange/postman-stackexchange-posts-api/)
- …and 7 more published on APIs.io

#### Governance rules (3)

Spectral rulesets for the provider's contracts.

- [Stack Exchange — jsonschema rules](https://apis.io/rules/stackexchange/stackexchange-jsonschema-spectral-rules/)
- [Stack Exchange API Rules](https://apis.io/rules/stackexchange/stackexchange-rules/)
- [Stack Exchange API Rules](https://apis.io/rules/stackexchange/stackexchange-spectral-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Stackexchange Authentication](https://apis.io/security/stackexchange/stackexchange-authentication/)
- [Stackexchange Domain Security](https://apis.io/security/stackexchange/stackexchange-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Stackexchange Scopes](https://apis.io/scopes/stackexchange/stackexchange-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Stackexchange Plans Pricing](https://apis.io/plans/stackexchange/stackexchange-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Stackexchange Rate Limits](https://apis.io/rate-limits/stackexchange/stackexchange-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://stackexchange.com/)
- [Documentation](https://api.stackexchange.com/docs)
- [Blog](https://stackoverflow.blog/)
- [Terms of service](https://stackoverflow.com/legal/api-terms-of-use)
- [Privacy policy](https://stackoverflow.com/legal/privacy-policy)
- [GitHub](https://github.com/StackExchange)
- [Status](https://stackstatus.tumblr.com/)

## API Evangelist rating

**Kin Score 41.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 20.8 |
| Contract governance | 27.3 |
| Operational transparency | 26.3 |
| Developer ergonomics | 51.2 |
| Access clarity | 42.1 |

**Agent readiness 30.5** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 34.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/stackexchange/](https://apis.io/providers/stackexchange/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Stack Exchange: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/stackexchange/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
