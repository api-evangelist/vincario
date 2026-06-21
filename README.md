# Vincario (vincario)

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
