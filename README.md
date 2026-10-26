# Gadjah Mada University (gadjah-mada-university)

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

Gadjah Mada University (Universitas Gadjah Mada, UGM) is a public research university in Yogyakarta, Indonesia, founded in 1949 and ranked #239 in the QS World University Rankings 2025. This repository catalogs UGM's public developer/API footprint as an [APIs.json](https://apisjson.org) profile.

Re-profiled 2026-09-01 under the API Evangelist university pipeline. UGM turns out to be one of the few institutions in this cohort that publishes a first-party API contract of its own: an **OpenAPI 3.1.0 document for UGM ID**, its OAuth 2.0 / OpenID Connect authorization server, served from its own host behind its own Swagger UI. Around it sit a self-published Shibboleth SAML 2.0 Identity Provider, a CAS server, and two independent, fully functional OAI-PMH 2.0 endpoints. What UGM does not have is a developer programme: no portal, no self-service registration, no changelog, no status page, no terms of service.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=gadjah-mada-university-api-evangelist&utm_content=repo

## Type

- University / Public Research University / Index / Consumer / 3rd-Party

## Tags

University, Higher Education, Education, Indonesia, Research, Identity Federation, Authentication, OpenID Connect, OAuth, Research Repository, Scholarly Publishing, OAI-PMH, Library

## APIs

Every entry carries an `x-operator` settled before any artifact was saved. `institution` means UGM runs the thing the surface describes; `registry` means UGM is registered in it, which is a fact about the institution and not a contract it wrote.

- **UGM ID — OAuth 2.0 / OpenID Connect Authorization Server** (`institution`) — UGM's own identity API, operated by DTI in front of SIMASTER. 20 operations, OIDC Discovery + RFC 8414 metadata, PKCE, RFC 7662 introspection, RFC 7009 revocation, RFC 8693 token exchange, public health check. Spec: https://oauth.simaster.ugm.ac.id/openapi.json — Docs: https://oauth.simaster.ugm.ac.id/docs — Base: https://oauth.simaster.ugm.ac.id
- **UGM Shibboleth SAML 2.0 Identity Provider** (`institution`) — entityID `https://sso.ugm.ac.id/idp/shibboleth`, self-published EntityDescriptor. Base: https://sso.ugm.ac.id/idp/profile/Metadata/SAML
- **UGM Institutional Repository OAI-PMH** (`institution`) — "repository civitas UGM", EPrints 3.3.15, six metadata prefixes. Base: http://repository.ugm.ac.id/cgi/oai2
- **UGM Journals OAI-PMH** (`institution`) — "Jurnal Universitas Gadjah Mada", Open Journal Systems, 100+ journal sets, DOIs under UGM's own Crossref prefix. Base: https://journal.ugm.ac.id/index/oai
- **UGM Single Sign-On (CAS)** (`institution`) — Base: https://sso.ugm.ac.id/cas
- **eLOK Moodle Web Services** (`institution` deployment, Moodle's contract) — self-hosted Moodle with web services enabled and token-gated. No Moodle specification is held here. Base: https://elok.ugm.ac.id/webservice/rest/server.php
- **Crossref membership** (`registry`) — member 9411, DOI prefix 10.22146.
- **ROR organization record** (`registry`) — https://ror.org/03ke6d638

## Artifacts

- OpenAPI: [openapi/](openapi/) — one searched (UGM's own, pristine copy in `openapi/_original/`) and two derived OAI-PMH contracts
- [authentication/](authentication/) — three identity stacks, plus UGM's SAML EntityDescriptor
- [scopes/](scopes/) · [json-schema/](json-schema/) · [examples/](examples/) · [errors/](errors/)
- [conformance/](conformance/) — the `education` regime's 12 domain standards, probed
- [lifecycle/](lifecycle/) · [rules/](rules/) · [vocabulary/](vocabulary/)
- [plans/](plans/gadjah-mada-university-plans-pricing.yml) · [rate-limits/](rate-limits/gadjah-mada-university-rate-limits.yml) · [finops/](finops/gadjah-mada-university-finops.yml)

## Domain standard conformance (education regime)

Four of twelve evidenced against a fetched artifact: **oai-pmh**, **saml**, **shibboleth**, **crossref**. Not found: scim, lti, oneroster, ed-fi, caliper, qti, orcid, datacite. Nothing was credited from a prose claim.

## Timestamps

- Created: 2026-06-03
- Modified: 2026-09-01

## Common Properties

- Website: https://ugm.ac.id/en/
- API Reference: https://oauth.simaster.ugm.ac.id/docs
- Status: https://oauth.simaster.ugm.ac.id/health
- Privacy Policy: https://ugm.ac.id/en/privacy-policy/
- Identity Federation: https://sso.ugm.ac.id/idp/profile/Metadata/SAML
- Research Repository: http://repository.ugm.ac.id/
- Scholarly Publishing: https://journal.ugm.ac.id/
- Library Catalog: https://opac.lib.ugm.ac.id/
- AI Policy: https://web.ugm.ac.id/etika-penggunaan-ai/
- GitHub: https://github.com/ugm-ac-id (org exists, zero public repos)
- LinkedIn: https://www.linkedin.com/school/universitas-gadjah-mada/
- Review: [review.yml](review.yml)

## Notes

Every URL in this profile was probed directly on 2026-09-01 and the full status-coded evidence table is in `x-coverage.evidence` in [apis.yml](apis.yml). Findings recorded rather than smoothed over:

- UGM's own OIDC and RFC 8414 discovery documents emit **scheme-less URLs** (`oauth.simaster.ugm.ac.id/oauth/token`), which both specifications forbid.
- The JWKS endpoint returns **200 with an empty key set** while advertising RS256 id_tokens.
- `https://repository.ugm.ac.id` returns **403** while `http://` returns **200**, so pointers to the repository are deliberately `http://`.
- The Shibboleth IdP declares `shibmd:Scope` as **`ac.id`** rather than `ugm.ac.id`, and is **absent from eduGAIN** (10,616 entities checked) — self-published, not inter-federated.
- The journal platform runs **OJS 2.4.8.1**, an end-of-life line, with a partial migration to OJS 3 under way and no published schedule.
- `data.ugm.ac.id` returns **HTTP 200 serving a maintenance page** — a soft-404. There is no open data portal. `api.ugm.ac.id` and `hpc.ugm.ac.id` do not resolve. `ai.ugm.ac.id` 502s. The student-run `opendata.bemkm.ugm.ac.id` returns 200 with a **zero-byte body**.
- The whole `/.well-known/` path on ugm.ac.id is **403'd at the edge**, so the absence of `security.txt` cannot be distinguished from a block.
- The main site's WordPress REST API returns a machine-readable **401 refusal** — a closed surface, not an API.

No vendor contract was found in this repository and none was added; nothing was removed. Only ONE contract is credited to UGM as authored — the UGM ID OpenAPI, which UGM publishes itself. The two OAI-PMH OpenAPIs are marked `method: derived` and are ours. No EPrints, OJS/PKP or Moodle product specification is held under this slug. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
