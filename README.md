# Western University (western)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
