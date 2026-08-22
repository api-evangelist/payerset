# Payerset (payerset)

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

Payerset is a healthcare price transparency data company that parses every payer Transparency in Coverage (TiC) machine-readable file and compliant hospital MRF each quarter, enriches negotiated rates with provider, payer, and claims metadata, and delivers it as analytics-ready datasets. The Payerset Data Lake API exposes payer-provider negotiated rate lookups, NPI/TIN provider mapping, billing-code classification, and hospital MRF discovery via a REST API authenticated with an x-api-key header.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/apis.yml)

## Tags

- Healthcare
- Price Transparency
- Negotiated Rates
- Machine-Readable Files
- Payer Data

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Payerset Negotiated Rates

Returns the payer-provider negotiated rate for a given billing code, payer, and provider NPI, derived from payer Transparency in Coverage machine-readable files (GET /v1/rates/rate_query).

- **Human URL:** [https://docs.payerset.com/data-lake/data-dictionary/payer-transparency-tic](https://docs.payerset.com/data-lake/data-dictionary/payer-transparency-tic)
- **Base URL:** `https://api.payerset.com`

#### Tags

- Negotiated Rates
- Rates
- Transparency in Coverage

#### Properties

- [Documentation](https://docs.payerset.com/data-lake/data-dictionary/payer-transparency-tic)
- [OpenAPI](openapi/payerset-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/payerset.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/payerset.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Payerset Rate Search

Reference-data search endpoints used to resolve a rate query - payer listings and detail, provider NPI detail, NPI/TIN/parent mappings, and billing-code detail and code types across the Data Lake.

- **Human URL:** [https://docs.payerset.com](https://docs.payerset.com)
- **Base URL:** `https://api.payerset.com`

#### Tags

- Rate Search
- Providers
- Payers
- Billing Codes

#### Properties

- [Documentation](https://docs.payerset.com)
- [OpenAPI](openapi/payerset-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/payerset.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/payerset.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Payerset Datasets

Dataset discovery and reference endpoints powering the Payerset Data Lake - hospital MRF hospital, system, and payer lists, plus provider EIN/TIN/NPI mapping and billing-code classification datasets, also delivered via S3 and Snowflake Marketplace.

- **Human URL:** [https://payerset.com/datalake/](https://payerset.com/datalake/)
- **Base URL:** `https://api.payerset.com`

#### Tags

- Datasets
- Data Lake
- Hospital MRF
- Mappings

#### Properties

- [Documentation](https://payerset.com/datalake/)
- [OpenAPI](openapi/payerset-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/payerset.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/payerset.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Payerset Benchmarks

Reimbursement benchmarking built on Payerset negotiated-rate data, comparing payer-provider rates across payers, providers, and billing codes. Surfaced through the Rate Explorer platform and Data Lake; no dedicated public benchmark API endpoint is documented in the published API definition.

- **Human URL:** [https://payerset.com/rateexplorer/](https://payerset.com/rateexplorer/)
- **Base URL:** `https://api.payerset.com`

#### Tags

- Benchmarks
- Reimbursement
- Market Analysis

#### Properties

- [Documentation](https://payerset.com/rateexplorer/)
- [OpenAPI](openapi/payerset-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/payerset.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/payerset.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/payerset)
- [LinkedIn](https://www.linkedin.com/company/payerset)
- [Website](https://www.payerset.com)
- [Documentation](https://docs.payerset.com)
- [Plans](plans/payerset-plans-pricing.yml)
- [Rate Limits](rate-limits/payerset-rate-limits.yml)
- [Fin Ops](finops/payerset-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
