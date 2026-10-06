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

Vincario (vincario.com, formerly vindecoder.eu) provides a REST API, currently version 3.2, that decodes a Vehicle Identification Number (VIN) into a vehicle specification and provides OEM VIN lookup, OEM service history, vehicle market value, stolen-vehicle checks, value lists (enums) for makes, models and other attributes, and the account credit balance. Requests are authenticated with an API key plus a control sum in the URL path. Vincario also runs a public MCP server (com.vincario/vehicle-data) and offers VIN OCR scanning and UK license plate lookup services, whose APIs are not yet publicly documented.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/apis.yml)

## Tags

- VIN
- Vehicle Data
- Automotive
- VIN Decoder
- Market Value

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-10-06

## APIs

### Vincario VIN Decoder API

Decode a VIN into a vehicle specification (VIN Decode) and list which fields can be decoded for a VIN (VIN Decode Info).

- **Human URL:** [https://vincario.com/vin-decoder/](https://vincario.com/vin-decoder/)
- **Base URL:** `https://api.vincario.com/3.2`

#### Tags

- VIN Decoder

#### Properties

- [OpenAPI](openapi/vincario-vin-decoder-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-VIN_Decoder-VIN_Decode)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-VIN_Decoder-VIN_Decode_Info)
- [API Reference](https://vincario.com/api-docs/3.2/)
- [Website](https://vincario.com/vin-decoder/)

### Vincario OEM VIN Lookup API

Look up manufacturer (OEM) data for a VIN.

- **Human URL:** [https://vincario.com/api-docs/3.2/#operations-OEM_VIN_Lookup-OEM_VIN_Lookup](https://vincario.com/api-docs/3.2/#operations-OEM_VIN_Lookup-OEM_VIN_Lookup)
- **Base URL:** `https://api.vincario.com/3.2`

#### Tags

- OEM VIN Lookup

#### Properties

- [OpenAPI](openapi/vincario-oem-vin-lookup-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-OEM_VIN_Lookup-OEM_VIN_Lookup)
- [API Reference](https://vincario.com/api-docs/3.2/)

### Vincario OEM Service History API

Retrieve manufacturer (OEM) service history for a VIN.

- **Human URL:** [https://vincario.com/api-docs/3.2/#operations-OEM_Service_History-OEM_Service_History](https://vincario.com/api-docs/3.2/#operations-OEM_Service_History-OEM_Service_History)
- **Base URL:** `https://api.vincario.com/3.2`

#### Tags

- OEM Service History

#### Properties

- [OpenAPI](openapi/vincario-oem-service-history-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-OEM_Service_History-OEM_Service_History)
- [API Reference](https://vincario.com/api-docs/3.2/)

### Vincario Vehicle Market Value API

Estimate the market value of a vehicle by VIN.

- **Human URL:** [https://vincario.com/vehicle-market-value/](https://vincario.com/vehicle-market-value/)
- **Base URL:** `https://api.vincario.com/3.2`

#### Tags

- Market Value

#### Properties

- [OpenAPI](openapi/vincario-vehicle-market-value-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Vehicle_Market_Value-Vehicle_Market_Value)
- [API Reference](https://vincario.com/api-docs/3.2/)
- [Website](https://vincario.com/vehicle-market-value/)

### Vincario Stolen Check API

Check whether a VIN appears in supported stolen-vehicle databases.

- **Human URL:** [https://vincario.com/stolen-vehicle-check/](https://vincario.com/stolen-vehicle-check/)
- **Base URL:** `https://api.vincario.com/3.2`

#### Tags

- Stolen Check

#### Properties

- [OpenAPI](openapi/vincario-stolen-check-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Stolen_Check-Stolen_Check)
- [API Reference](https://vincario.com/api-docs/3.2/)
- [Website](https://vincario.com/stolen-vehicle-check/)

### Vincario Credit Balance API

Return the remaining credit balance of the account.

- **Human URL:** [https://vincario.com/api-docs/3.2/#operations-Get_Balance-Get_Balance](https://vincario.com/api-docs/3.2/#operations-Get_Balance-Get_Balance)
- **Base URL:** `https://api.vincario.com/3.2`

#### Tags

- Account

#### Properties

- [OpenAPI](openapi/vincario-get-balance-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Get_Balance-Get_Balance)
- [API Reference](https://vincario.com/api-docs/3.2/)

### Vincario Enums API

Value lists for vehicle makes, models, make and model combinations, body, color, drive, fuel, product type and transmission.

- **Human URL:** [https://vincario.com/api-docs/3.2/#operations-Enums-Enum_Make](https://vincario.com/api-docs/3.2/#operations-Enums-Enum_Make)
- **Base URL:** `https://api.vincario.com/3.2`

#### Tags

- Enums

#### Properties

- [OpenAPI](openapi/vincario-enums-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Enums-Enum_Make)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Enums-Enum_Model)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Enums-Enum_Vehicle)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Enums-Enum_Body)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Enums-Enum_Color)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Enums-Enum_Drive)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Enums-Enum_Fuel)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Enums-Enum_Product_Type)
- [Documentation](https://vincario.com/api-docs/3.2/#operations-Enums-Enum_Transmission)
- [API Reference](https://vincario.com/api-docs/3.2/)

## Authentication

Every request is a GET against `https://api.vincario.com/3.2/{API_KEY}/{CONTROL_SUM}/...` that carries the API key and a per-request control sum as path segments. Per the provider's OpenAPI, the control sum is the first 10 characters of the SHA1 hash of the lookup value (for example the VIN), the operation id (for example `decode`), the API key and the secret key, pipe-delimited in that order. The secret key is never transmitted.

## Common Properties

- [AgenticAccess](agentic-access/vincario-agentic-access.yml)
- [VulnerabilityDisclosure](security/vincario-vulnerability-disclosure.yml)
- [DomainSecurity](security/vincario-domain-security.yml)
- [Authentication](authentication/vincario-authentication.yml)
- [LinkedIn](https://www.linkedin.com/company/vincario)
- [Website](https://vincario.com)
- [Documentation](https://vincario.com/api-docs/)
- [APIReference](https://vincario.com/api-docs/3.2/)
- [Vincario API 3.2 OpenAPI (provider-published, saved verbatim in openapi/_original/vincario-openapi.yml)](https://vincario.com/api-docs/openapi/3.2)
- [Vincario MCP server (com.vincario/vehicle-data, https://mcp.vincario.com/mcp)](mcp/vincario-mcp.yml)
- [GitHubRepository](https://github.com/Vincario/MCP-vincario)
- [VIN OCR Scanner (API exists; public API documentation not yet published)](https://vincario.com/vin-ocr-scanner/)
- [License Plate Lookup (UK registration plates)](https://vincario.com/license-plate-lookup/)
- [Plans](plans/vincario-plans-pricing.yml)
- [RateLimits](rate-limits/vincario-rate-limits.yml)
- [FinOps](finops/vincario-finops.yml)
- [Blog](https://vincario.com/blog/feed/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
