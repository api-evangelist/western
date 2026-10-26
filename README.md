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

Western University is a public research university in London, Ontario, Canada, ranked #120 in the QS World University Rankings 2025. This repository catalogs Western's public developer and API footprint as an [APIs.json](https://apisjson.org) profile. Western is a federation of buyers, not an API producer: the one class of machine-readable surface it operates itself is **identity** — a Shibboleth Identity Provider registered in the Canadian Access Federation and exported to eduGAIN, plus an Apereo CAS server with a live CAS 3.0 validation endpoint. Everything else readable here is a **tenancy** on a platform someone else runs — Scholarship@Western on Scholars Portal's national Scholaris DSpace service, Western's research data on Borealis, and library discovery on OCUL's shared Ex Libris Primo VE — recorded as relationships, with no vendor contract saved under Western's name.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/western/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=western-api-evangelist&utm_content=repo

## Type

- **Class:** university (`x-type: university`)
- **Category:** Public Research University
- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

University, Higher Education, Education, Research, Canada, Ontario, U15, Identity Federation, Research Repository, Research Data, Open Access, OAI-PMH, Library

## APIs

Every surface carries an `x-operator`: **institution** means Western runs the thing the contract describes, **tenant** means Western owns the account and the content but a vendor wrote and runs the contract.

- **Western University Shibboleth Identity Provider (SAML 2.0)** — *institution*. entityID `https://shibidp.uwo.ca/idp/shibboleth`, registered in the Canadian Access Federation by CANARIE since 2012, exported to eduGAIN, declaring REFEDS Research & Scholarship and Sirtfi. Metadata: https://caf-shib2ops.ca/CoreServices/caf_metadata_signed_sha256.xml
- **Western Single Sign-On (Apereo CAS — CAS 3.0, SAML2, OIDC)** — *institution*. https://ssocas.uwo.ca/cas · SAML descriptor https://ssocas.uwo.ca/cas/idp/metadata · OIDC advertised but discovery returns 403.
- **Scholarship@Western on Scholaris — DSpace REST API** — *tenant* (Scholars Portal / OCUL, DSpace 8.4). https://uwo.scholaris.ca/server/api
- **Scholarship@Western OAI-PMH 2.0** — *tenant*. https://uwo.scholaris.ca/server/oai/request?verb=Identify · 13 metadata formats.
- **Western University Repository on Borealis — Dataverse API** — *tenant* (Scholars Portal, Dataverse 6.8.4). https://borealisdata.ca/api/dataverses/westernu · 1,504 datasets, DataCite DOIs on prefix 10.5683.
- **Omni library discovery — Ex Libris Primo VE** — *tenant* (Ex Libris via OCUL). No contract saved.

## Plans, Rate Limits, and FinOps

- Plans & Pricing: [plans/western-plans-pricing.yml](plans/western-plans-pricing.yml)
- Rate Limits: [rate-limits/western-rate-limits.yml](rate-limits/western-rate-limits.yml)
- FinOps: [finops/western-finops.yml](finops/western-finops.yml)

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-08-30

## Common Properties

- Website: https://www.uwo.ca/
- Documentation: https://wts.uwo.ca/services/index.html
- Support: https://wts.uwo.ca/
- Privacy Policy: https://www.uwo.ca/legalcounsel/privacy/
- Blog: https://news.westernu.ca/ · RSS: https://news.westernu.ca/feed
- LinkedIn: https://ca.linkedin.com/school/westernuniversity/
- Twitter/X: https://x.com/westernu
- Identity Federation: https://ssocas.uwo.ca/cas/idp/metadata
- Research Repository: https://uwo.scholaris.ca/home
- Library Catalog: https://ocul-uwo.primo.exlibrisgroup.com/discovery/search?vid=01OCUL_UWO:UWO_DEFAULT
- Course Catalog: https://westerncalendar.uwo.ca/
- AI Policy: https://ai.uwo.ca/governance/policies.html
- AI Tooling: https://ai.uwo.ca/resources/ai-tools.html
- Authentication: [authentication/western-authentication.yml](authentication/western-authentication.yml)
- Conformance: [conformance/western-conformance.yml](conformance/western-conformance.yml)

## Notes

Re-profiled 2026-08-30 under the API Evangelist university pipeline, which settles **who operates each surface** before saving anything. Nothing was fabricated; every claim above is backed by a live probe recorded in [conformance/western-conformance.yml](conformance/western-conformance.yml), [authentication/western-authentication.yml](authentication/western-authentication.yml) and the `x-coverage` block in `apis.yml`.

What changed from the 2026-06-03 profile:

- **Found:** Western's Shibboleth IdP in the Canadian Access Federation aggregate — the most consequential machine-readable surface Western publishes, and absent from the original profile.
- **Found:** Western's 1,504-dataset research data collection on Borealis, absent from the original profile.
- **Recorded:** the OAI-PMH provider as an API entry (it was documented in this README but never in `apis.yml`).
- **Relabelled:** Scholaris and Omni from implied Western surfaces to explicit **tenant** relationships.
- **Corrected:** Scholaris reports DSpace **8.4**, not 8.3.

Deliberate exclusions: `api.uwo.ca` and `developer.uwo.ca` do not resolve. `data.uwo.ca` resolves but redirects to the Office of Institutional Planning & Budgeting — HTML dashboards, no API — so it is not recorded as an open-data surface. The GitHub organisations `western-university` and `uwo-ca` both exist but hold zero public repositories and no identifying metadata, so neither can be attributed to Western and no GitHub pointer is emitted. There is no official course, timetable or open-data API: `westerncalendar.uwo.ca` blocks ClaudeBot, GPTBot, PerplexityBot, OAI-SearchBot, Applebot, Amazonbot, Googlebot and bingbot in `robots.txt`, the undergraduate timetable is scrape-only, and the only APIs over that data are unofficial student projects on non-Western domains that Western does not endorse. Western serves no `llms.txt` and no `.well-known/security.txt`. ORCID integration is present in the DSpace software but unconfigured on Western's instance.

See [review.yml](review.yml) for the 2026-06-03 per-endpoint verification.

## Maintainers

- Kin Lane — kin@apievangelist.com
