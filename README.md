# Western University (western)

Western University is a public research university in London, Ontario, Canada, ranked #120 in the QS World University Rankings 2025. This repository catalogs Western's public developer and API footprint as an [APIs.json](https://apisjson.org) profile. Western's machine-readable surface is centered on Western Libraries — the Scholarship@Western institutional repository, which migrated in 2025 to the national Scholaris DSpace 8 service (live REST API + OAI-PMH) — plus an affiliation-gated institutional Single Sign-On service from Western Technology Services.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/western/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=western-api-evangelist&utm_content=repo

## Type

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Education, Higher Education, University, Canada, Library, Institutional Repository, Open Access, Identity

## APIs

- **Scholaris (Scholarship@Western) DSpace REST API** — DSpace 8.3 REST (HAL) API for Western's Open Repository. Docs: https://uwo.scholaris.ca/home · API root: https://uwo.scholaris.ca/server/api
- **Scholarship@Western OAI-PMH** — OAI-PMH 2.0 metadata harvesting for the institutional repository. Endpoint: https://uwo.scholaris.ca/server/oai/request?verb=Identify · Docs: https://ir.lib.uwo.ca/about.html
- **Western Single Sign-On (SAML2 / OAuth / OIDC / CAS)** — WTS institutional SSO; request-based and affiliation-gated. Docs: https://wts.uwo.ca/services/o/single-sign-on-sso-saml2-oauth-oidc-cas/index.html

## Plans, Rate Limits, and FinOps

- Plans & Pricing: [plans/western-plans-pricing.yml](plans/western-plans-pricing.yml)
- Rate Limits: [rate-limits/western-rate-limits.yml](rate-limits/western-rate-limits.yml)
- FinOps: [finops/western-finops.yml](finops/western-finops.yml)

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-06-03

## Common Properties

- Website: https://www.uwo.ca/
- LinkedIn: https://ca.linkedin.com/school/westernuniversity/
- Twitter/X: https://x.com/westernu
- Authentication: https://wts.uwo.ca/services/o/single-sign-on-sso-saml2-oauth-oidc-cas/index.html

## Notes

All APIs, endpoints, and properties listed here were verified live as of 2026-06-03; nothing was fabricated. The DSpace REST API root and OAI-PMH endpoint return valid responses (DSpace 8.3). Western does **not** publish an official open course/timetable or open-data API — timetable data is documented only as scrape targets with an unofficial third-party API on GitHub. There is **no** official Western University GitHub organization (the `uwo` GitHub account is an unrelated personal user), so no GitHub common property is listed. The SSO service is documented but request-based and gated behind institutional affiliation. See [review.yml](review.yml) for per-endpoint verification details.

## Maintainers

- Kin Lane — kin@apievangelist.com
