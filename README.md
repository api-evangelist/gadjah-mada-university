# Gadjah Mada University

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

Gadjah Mada University (Universitas Gadjah Mada, UGM) is a public research university in Yogyakarta, Indonesia, founded in 1949 and the country's oldest and largest state university. Unusually for this cohort, UGM's programmable footprint is real and it is its own: the university operates and publishes a first-party OpenAPI 3.1.0 contract for UGM ID, its OAuth 2.0 / OpenID Connect authorization server at oauth.simaster.ugm.ac.id, complete with an OIDC Discovery document, an RFC 8414 authorization-server metadata document, PKCE, RFC 7662 introspection, RFC 7009 revocation, RFC 8693 token exchange, a Swagger UI and a public health endpoint. Alongside it UGM runs its own Shibboleth SAML 2.0 Identity Provider, a CAS server, and two independent, fully functional OAI-PMH 2.0 endpoints — the EPrints institutional repository at repository.ugm.ac.id and the university-wide Open Journal Systems platform at journal.ugm.ac.id, whose articles carry DOIs under UGM's own Crossref prefix 10.22146 (member 9411). None of that is a vendor's contract running under UGM's name; every host is under ugm.ac.id and every specification describes itself as UGM's. What UGM does not have is a developer programme. There is no developer portal, no self-service client registration, no dynamic client registration, no documented route to a client_id, no changelog, no status page, no terms of service and no licence on any surface. There is no open data portal — data.ugm.ac.id returns a maintenance page — no public course, timetable or registrar API, and no research-computing service catalog. The main site's WordPress REST API is deliberately closed to anonymous callers, and the whole /.well-known/ path is blocked at the edge. The honest summary is a genuine engineering surface with no consumer-facing programme around it, plus three real registry and federation relationships recorded as facts about the institution rather than as contracts it wrote.

**Areas:** University · Higher Education · Education · Indonesia · Research · Identity Federation · Authentication · Research Repository · Scholarly Publishing · OAI-PMH · Library

## Gadjah Mada University on APIs.io

Everything profiled for Gadjah Mada University is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/gadjah-mada-university/](https://apis.io/providers/gadjah-mada-university/)** — or go straight to one of the APIs or properties below.

### APIs (12)

- [UGM Shibboleth SAML 2.0 Identity Provider](https://apis.io/apis/gadjah-mada-university/shibboleth-idp/) — UGM's own Shibboleth Identity Provider, entityID https://sso.ugm.ac.id/idp/shibboleth, publishing an unsigned SAML EntityDescriptor from the university's…
- [UGM Single Sign-On (CAS)](https://apis.io/apis/gadjah-mada-university/sso-cas/) — Central Authentication Service at sso.ugm.ac.id/cas, the login surface UGM systems redirect users to. A bare GET redirects to /cas/login and returns the…
- [eLOK Moodle Web Services (institution deployment)](https://apis.io/apis/gadjah-mada-university/elok-moodle-webservices/) — UGM's self-hosted Moodle learning platform, eLOK, at elok.ugm.ac.id, with Moodle Web Services enabled and token-gated. Verified live on 2026-09-01:…
- [Crossref membership (member 9411, prefix 10.22146)](https://apis.io/apis/gadjah-mada-university/crossref-membership/) — Universitas Gadjah Mada is a Crossref member in its own name — member id 9411, DOI prefix 10.22146 — verified live on 2026-09-01 against the Crossref REST…
- [ROR organization record (ror.org/03ke6d638)](https://apis.io/apis/gadjah-mada-university/ror-record/) — Universitas Gadjah Mada's Research Organization Registry identifier, https://ror.org/03ke6d638, verified live on 2026-09-01 against the ROR v2 API. The…
- [Gadjah Mada University Discovery API](https://apis.io/apis/gadjah-mada-university/gadjah-mada-university-discovery-api/) — RFC 8414 & OIDC Discovery
- [Gadjah Mada University Infra API](https://apis.io/apis/gadjah-mada-university/gadjah-mada-university-infra-api/) — Health check & infrastruktur
- [Gadjah Mada University OAI PMH API](https://apis.io/apis/gadjah-mada-university/gadjah-mada-university-oai-pmh-api/) — Open Archives Initiative Protocol for Metadata Harvesting, version 2.0.
- [Gadjah Mada University Social Login API](https://apis.io/apis/gadjah-mada-university/gadjah-mada-university-social-login-api/) — Social provider login (Google, Microsoft, Facebook, LinkedIn)
- [Gadjah Mada University O Auth2 API](https://apis.io/apis/gadjah-mada-university/gadjah-mada-university-oauth2-api/) — Endpoint inti OAuth2/OIDC
- [Gadjah Mada University Me API](https://apis.io/apis/gadjah-mada-university/gadjah-mada-university-me-api/) — The Me API from Gadjah Mada University — 1 operation(s) for me.
- [Gadjah Mada University User API](https://apis.io/apis/gadjah-mada-university/gadjah-mada-university-user-api/) — The User API from Gadjah Mada University — 2 operation(s) for user.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Gadjah Mada University Agentic Access](https://apis.io/agentic-access/gadjah-mada-university/gadjah-mada-university-agentic-access/)

#### JSON Schema (1)

The data models the API reads and writes.

- [UGM ID — JSON Schemas](https://apis.io/schemas/gadjah-mada-university/gadjah-mada-university-ugm-id-schemas/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Gadjah Mada University Context](https://apis.io/jsonld/gadjah-mada-university/gadjah-mada-university-context/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Gadjah Mada University API Rules](https://apis.io/rules/gadjah-mada-university/gadjah-mada-university-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Gadjah Mada University Authentication](https://apis.io/security/gadjah-mada-university/gadjah-mada-university-authentication/)
- [Gadjah Mada University Domain Security](https://apis.io/security/gadjah-mada-university/gadjah-mada-university-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Gadjah Mada University Scopes](https://apis.io/scopes/gadjah-mada-university/gadjah-mada-university-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Gadjah Mada University Plans Pricing](https://apis.io/plans/gadjah-mada-university/gadjah-mada-university-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Gadjah Mada University Rate Limits](https://apis.io/rate-limits/gadjah-mada-university/gadjah-mada-university-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Gadjah Mada University Finops](https://apis.io/finops/gadjah-mada-university/gadjah-mada-university-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://ugm.ac.id/en/)
- [Documentation](https://oauth.simaster.ugm.ac.id/openapi.json)
- [API reference](https://oauth.simaster.ugm.ac.id/docs)
- [Support](https://dti.ugm.ac.id/knowledge-base/)
- [Blog](https://ugm.ac.id/en/news/)
- [Privacy policy](https://ugm.ac.id/en/privacy-policy/)

## API Evangelist rating

**Kin Score 38.6** — thin · rubric 0.24.0 · scored 2026-10-20

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 58.8 |
| Contract governance | 33.3 |
| Operational transparency | 10.5 |
| Developer ergonomics | 35.7 |
| Access clarity | 15.8 |

**Agent readiness 28.9** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | unknown |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 30.4** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/gadjah-mada-university/](https://apis.io/providers/gadjah-mada-university/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Gadjah Mada University: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/gadjah-mada-university/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
