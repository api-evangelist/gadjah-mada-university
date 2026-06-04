# Gadjah Mada University (gadjah-mada-university)

Gadjah Mada University (Universitas Gadjah Mada, UGM) is a public research university in Yogyakarta, Indonesia, ranked #239 in the QS World University Rankings 2025. This repository catalogs UGM's public developer/API footprint as an [APIs.json](https://apisjson.org) profile. That footprint is limited: the most concrete public, no-auth API is the institutional repository's OAI-PMH endpoint, alongside a centralized CAS single sign-on service.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=gadjah-mada-university-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Indonesia, Research, Open Data, Library, Repository

## APIs

- **UGM Repository OAI-PMH** — OAI-PMH 2.0 metadata harvesting for the EPrints institutional repository ("repository civitas UGM"). Docs: http://repository.ugm.ac.id/information.html — Base: http://repository.ugm.ac.id/cgi/oai2
- **UGM Single Sign-On (CAS)** — Central Authentication Service used across UGM systems; credential-gated authentication service. Docs: https://dti.ugm.ac.id/knowledge-base/akses-365 — Base: https://sso.ugm.ac.id/cas

## Plans

- [plans/gadjah-mada-university-plans-pricing.yml](plans/gadjah-mada-university-plans-pricing.yml)

## Rate Limits

- [rate-limits/gadjah-mada-university-rate-limits.yml](rate-limits/gadjah-mada-university-rate-limits.yml)

## FinOps

- [finops/gadjah-mada-university-finops.yml](finops/gadjah-mada-university-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://ugm.ac.id/en/
- GitHub: https://github.com/ugm-ac-id (org exists, no public repos)
- LinkedIn: https://www.linkedin.com/school/universitas-gadjah-mada/
- Review: [review.yml](review.yml)

## Notes

All URLs in this profile were probed directly. The OAI-PMH endpoint was verified live via an `Identify` request (returns `repository civitas UGM`, EPrints, admin `library@ugm.ac.id`). The CAS login endpoint resolves (HTTP 200) but is an authentication service requiring valid UGM credentials, not an open data API. The ETD repository resolves but exposed no OAI endpoint at the standard path. A student-run (BEM KM) open-data portal at opendata.bemkm.ugm.ac.id resolves but publishes no documented public API. No official developer portal, REST API documentation, or public signup flow was found. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
