# Payerset (payerset)

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
