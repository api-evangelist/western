# Western University

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

Western University is a public research university in London, Ontario, Canada, ranked #120 in the QS World University Rankings order used by this cohort. Like almost every university, Western is a federation of buyers rather than an API producer: it runs no developer portal, no institutional API gateway (api.uwo.ca and developer.uwo.ca do not resolve), publishes no OpenAPI for anything, and serves no llms.txt or security.txt. What it genuinely operates is identity. Western Technology Services runs a Shibboleth Identity Provider, entityID https://shibidp.uwo.ca/idp/shibboleth, registered in the Canadian Access Federation since 2012 under CANARIE and exported to eduGAIN, declaring the REFEDS Research and Scholarship entity category and Sirtfi assurance — machine-readable SAML 2.0 metadata that is the single most consequential surface Western publishes. Alongside it runs an Apereo CAS server at ssocas.uwo.ca with a live CAS 3.0 validation endpoint and a second SAML descriptor whose entityID is still the stock Apereo placeholder. Both are end-user login federations, not developer authorization surfaces; OIDC is advertised by WTS but its discovery document returns 403. Western's two readable data surfaces are tenancies, not engineering: Scholarship@Western moved in 2025 to Scholaris, the national shared DSpace 8.4 service run by Scholars Portal (OCUL), exposing a HAL REST API and a conformant OAI-PMH 2.0 provider across thirteen metadata formats at uwo.scholaris.ca; and Western's research data lives in a 1,504-dataset collection on Borealis, the Canadian Dataverse Repository, minting DataCite DOIs on Scholars Portal's 10.5683 prefix. Library discovery is an Ex Libris Primo VE view on OCUL's shared platform. All four are recorded here as tenant relationships and deliberately not credited as Western engineering. There is no official course, timetable or open-data API: the academic calendar at westerncalendar.uwo.ca blocks every AI and search crawler in robots.txt, the undergraduate timetable is scrape-only, and the only APIs over that data are unofficial student projects on GitHub that Western does not endorse.

**Areas:** University · Higher Education · Education · Research · Canada · Ontario · U15 · Identity Federation · Research Repository · Research Data · Open Access · OAI-PMH

## Western University on APIs.io

Everything profiled for Western University is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/western/](https://apis.io/providers/western/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [Western University Shibboleth Identity Provider (SAML 2.0 metadata)](https://apis.io/apis/western/identity-federation/) — Western's institutional identity provider, publishing machine-readable SAML 2.0 metadata through the Canadian Access Federation. entityID…
- [Western Single Sign-On (Apereo CAS — CAS 3.0, SAML2, OIDC)](https://apis.io/apis/western/sso-cas/) — Western Technology Services operates an Apereo CAS server at ssocas.uwo.ca. The CAS 3.0 protocol is publicly reachable — /cas/p3/serviceValidate returns a…
- [Scholarship@Western on Scholaris — DSpace REST API (tenant)](https://apis.io/apis/western/scholaris-rest/) — The HAL+JSON REST API of Western University's Open Repository, reachable anonymously at https://uwo.scholaris.ca/server/api. The root document self-reports…
- [Scholarship@Western OAI-PMH 2.0 provider (tenant)](https://apis.io/apis/western/scholaris-oai-pmh/) — OAI-PMH 2.0 metadata harvesting for Western University's Open Repository. Identify returns repositoryName "Western University's Open Repository",…
- [Western University Repository on Borealis — Dataverse API (tenant)](https://apis.io/apis/western/borealis-dataverse/) — Western's research data repository, a Dataverse collection with alias "westernu" and affiliation "Western University" on Borealis, the Canadian Dataverse…
- [Omni library discovery — Ex Libris Primo VE (tenant)](https://apis.io/apis/western/omni-primo/) — Western Libraries' discovery layer is Omni, the Ontario Council of University Libraries' shared Ex Libris Alma/Primo VE deployment. Western's view is…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Western Context](https://apis.io/jsonld/western/western-context/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Western Authentication](https://apis.io/security/western/western-authentication/)
- [Western Domain Security](https://apis.io/security/western/western-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Western Plans Pricing](https://apis.io/plans/western/western-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Western Rate Limits](https://apis.io/rate-limits/western/western-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Western Finops](https://apis.io/finops/western/western-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.uwo.ca/)
- [Documentation](https://wts.uwo.ca/services/index.html)
- [Support](https://wts.uwo.ca/)
- [Blog](https://news.westernu.ca/)
- [Privacy policy](https://www.uwo.ca/legalcounsel/privacy/)

## API Evangelist rating

**Kin Score 23.8** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 62.5 |
| Contract quality | 20.4 |
| Contract governance | 0.0 |
| Operational transparency | 5.3 |
| Developer ergonomics | 35.7 |
| Access clarity | 15.8 |

**Agent readiness 4.4** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
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

**Regulatory alignment 28.4** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/western/](https://apis.io/providers/western/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Western University: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/western/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
