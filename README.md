# Vincario (vincario)

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

Vincario operates the vindecoder.eu VIN Decoder API, a global REST service that decodes a Vehicle Identification Number (VIN) into a full vehicle specification and provides vehicle market value, stolen-vehicle checks, and account balance. Requests are authenticated with an API key plus a SHA1 control sum embedded in the URL path.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/apis.yml)

## Tags

- VIN
- Vehicle Data
- Automotive
- VIN Decoder
- Market Value

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Vincario VIN Decode API

Decodes a 17-character VIN into a full vehicle specification (make, model, model year, body, engine, fuel, transmission and ~40 European-market data points) returned as JSON or HTML.

- **Human URL:** [https://vindecoder.eu/api](https://vindecoder.eu/api)
- **Base URL:** `https://api.vindecoder.eu/3.2`

#### Tags

- VIN
- Decode
- Vehicle Specification

#### Properties

- [Documentation](https://vindecoder.eu/api)
- [API Reference](https://vindecoder.eu/api)
- [OpenAPI](openapi/vincario-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vincario.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vincario.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vincario Vehicle Market Value API

Returns statistical market data (price and odometer) for vehicles matching a decoded VIN, including the input parameters used for the computation.

- **Human URL:** [https://vindecoder.eu/vehicle-market-value](https://vindecoder.eu/vehicle-market-value)
- **Base URL:** `https://api.vindecoder.eu/3.2`

#### Tags

- Market Value
- Pricing
- Valuation

#### Properties

- [Documentation](https://vindecoder.eu/vehicle-market-value)
- [OpenAPI](openapi/vincario-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vincario.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vincario.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vincario Stolen Check API

Performs a real-time check of a VIN against national police databases of stolen vehicles (Czech Republic, Hungary, Lithuania, Romania, Slovenia, Slovakia) and Vincario's own database of stolen vehicles.

- **Human URL:** [https://vindecoder.eu/api](https://vindecoder.eu/api)
- **Base URL:** `https://api.vindecoder.eu/3.2`

#### Tags

- Stolen Check
- Fraud
- Police Database

#### Properties

- [Documentation](https://vindecoder.eu/api)
- [OpenAPI](openapi/vincario-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vincario.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vincario.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vincario Vehicle Info API

Returns the list of vehicle details that can be decoded for a given VIN by the decode service; this informational lookup is free of charge.

- **Human URL:** [https://vindecoder.eu/api](https://vindecoder.eu/api)
- **Base URL:** `https://api.vindecoder.eu/3.2`

#### Tags

- Vehicle Info
- Metadata
- Capabilities

#### Properties

- [Documentation](https://vindecoder.eu/api)
- [OpenAPI](openapi/vincario-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vincario.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vincario.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vincario Account Balance API

Returns the remaining API credits/balance for each service on the authenticated account.

- **Human URL:** [https://vindecoder.eu/api](https://vindecoder.eu/api)
- **Base URL:** `https://api.vindecoder.eu/3.2`

#### Tags

- Account
- Balance
- Credits

#### Properties

- [Documentation](https://vindecoder.eu/api)
- [OpenAPI](openapi/vincario-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vincario.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vincario.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Authentication

Every request is a GET against a path that carries the API key (id) and a per-request control sum as path segments. The control sum is the first 10 characters of `sha1("{lookup}|{id}|{apikey}|{secretkey}")`, where `{lookup}` is the uppercased VIN for VIN-based endpoints (and the API key for the balance endpoint) and `{id}` is the endpoint identifier (`decode`, `vininfo`, `vehicle-market-value`, `stolencheck`, `balance`). The secret key is never transmitted — it is only used locally to derive the control sum. Path layout: `/{apikey}/{controlsum}/{id}/{vin}.json`.

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/vincario)
- [Website](https://vincario.com)
- [Documentation](https://vindecoder.eu/api)
- [Plans](plans/vincario-plans-pricing.yml)
- [Rate Limits](rate-limits/vincario-rate-limits.yml)
- [Fin Ops](finops/vincario-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
