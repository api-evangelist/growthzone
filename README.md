# GrowthZone (growthzone)

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

GrowthZone is association management software (AMS) for chambers of commerce, trade and professional associations, and member-based organizations - covering membership management, member and organization contacts, event registration, invoicing and scheduled billing, member directories, certifications, and communications. The GrowthZone REST API (base `https://{subdomain}.growthzoneapp.com/api`, where `{subdomain}` is your customer database sub-domain) exposes this data programmatically for CMS/directory embeds, single sign-on, and mobile integrations. GrowthZone also operates ChamberMaster and MemberZone, which expose a separate legacy REST API.

The API is **customer/partner-gated**: your account must have API Access enabled and an API Key issued by GrowthZone WebSupport (websupport@growthzone.com). Server authentication uses an `Authorization: ApiKey {API_Key}` header; OAuth 2.0 / OpenID Connect is supported for user (SSO) flows. The API is documented publicly at [integration.growthzone.com](https://integration.growthzone.com). Endpoints in this catalog are marked **Confirmed** (present in the public integration/Curated API docs) or **Modeled** (honestly inferred for standard CRUD or the ChamberMaster/MemberZone event feed).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/apis.yml)

## Tags

- Association Management
- AMS
- Membership Management
- Chambers of Commerce
- ChamberMaster
- Member Directory
- Events
- Billing

## Timestamps

- **Created:** 2026-07-05
- **Modified:** 2026-07-05

## APIs

### GrowthZone Contacts API

Retrieve and page contacts - both individuals (persons) and organizations - with related addresses, emails, websites, categories, notes/custom fields, group memberships, and a delta feed of contacts changed since a given date.

- **Human URL:** [https://integration.growthzone.com/growthzone-api/](https://integration.growthzone.com/growthzone-api/)
- **Base URL:** `https://{subdomain}.growthzoneapp.com/api`

#### Tags

- Contacts
- Members
- Organizations

#### Properties

- [Documentation](https://integration.growthzone.com/growthzone-api/)
- [API Reference](https://documentation.growthzoneapp.com/CuratedApi.html)
- [OpenAPI](openapi/growthzone-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/growthzone.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/growthzone.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GrowthZone Memberships API

List membership types and page all memberships (optionally filtered by type and membership status - Prospective, Active, Courtesy, NonMember, Inactive), including membership change events.

- **Human URL:** [https://integration.growthzone.com/growthzone-api/](https://integration.growthzone.com/growthzone-api/)
- **Base URL:** `https://{subdomain}.growthzoneapp.com/api`

#### Tags

- Memberships
- Membership Types
- Members

#### Properties

- [Documentation](https://integration.growthzone.com/growthzone-api/)
- [API Reference](https://documentation.growthzoneapp.com/CuratedApi.html)
- [OpenAPI](openapi/growthzone-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/growthzone.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/growthzone.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GrowthZone Groups & Directory API

Resolve groups by category and list group members, plus category summaries used to build searchable, category-filtered member directories embedded in a public website.

- **Human URL:** [https://integration.growthzone.com/growthzone-api/](https://integration.growthzone.com/growthzone-api/)
- **Base URL:** `https://{subdomain}.growthzoneapp.com/api`

#### Tags

- Groups
- Directory
- Categories

#### Properties

- [Documentation](https://integration.growthzone.com/growthzone-api/)
- [API Reference](https://documentation.growthzoneapp.com/CuratedApi.html)
- [OpenAPI](openapi/growthzone-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/growthzone.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/growthzone.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GrowthZone Scheduled Billing API

Preview, export, set up, and run scheduled recurring membership billing by membership type, and retrieve and download the history of past billing runs.

- **Human URL:** [https://documentation.growthzoneapp.com/ScheduledBilling.html](https://documentation.growthzoneapp.com/ScheduledBilling.html)
- **Base URL:** `https://{subdomain}.growthzoneapp.com/api`

#### Tags

- Billing
- Invoices
- Scheduled Billing

#### Properties

- [API Reference](https://documentation.growthzoneapp.com/ScheduledBilling.html)
- [OpenAPI](openapi/growthzone-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/growthzone.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/growthzone.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GrowthZone Certifications API

Mark certification components complete for a contact's certification track, supporting continuing-education and credentialing programs run inside GrowthZone.

- **Human URL:** [https://documentation.growthzoneapp.com/CuratedApi.html](https://documentation.growthzoneapp.com/CuratedApi.html)
- **Base URL:** `https://{subdomain}.growthzoneapp.com/api`

#### Tags

- Certifications
- Continuing Education

#### Properties

- [API Reference](https://documentation.growthzoneapp.com/CuratedApi.html)
- [OpenAPI](openapi/growthzone-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/growthzone.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/growthzone.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GrowthZone Events API

List and filter events by date range and status for embedding association event calendars into a website or mobile app. Modeled from GrowthZone's ChamberMaster/MemberZone event feed (legacy base `api.micronetonline.com/v1`); exact GrowthZone-native event paths are behind the gated reference.

- **Human URL:** [https://integration.growthzone.com/chambermaster-or-memberzone-api-documentation/](https://integration.growthzone.com/chambermaster-or-memberzone-api-documentation/)
- **Base URL:** `https://{subdomain}.growthzoneapp.com/api`

#### Tags

- Events
- Registration
- Calendar

#### Properties

- [Documentation](https://integration.growthzone.com/chambermaster-or-memberzone-api-documentation/)
- [OpenAPI](openapi/growthzone-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/growthzone.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/growthzone.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GrowthZone OAuth / OpenID Connect (SSO) API

OpenID Connect provider for single sign-on - authorize, token, userinfo, and JWKS endpoints supporting authorization-code, implicit, and hybrid flows with the `openid`, `profile`, and `email` scopes.

- **Human URL:** [https://integration.growthzone.com/growthzone-oauth-documentation/](https://integration.growthzone.com/growthzone-oauth-documentation/)
- **Base URL:** `https://growthzoneapp.com`

#### Tags

- OAuth
- OpenID Connect
- SSO
- Authentication

#### Properties

- [Documentation](https://integration.growthzone.com/growthzone-oauth-documentation/)
- [OpenAPI](openapi/growthzone-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/growthzone)
- [Website](https://www.growthzone.com)
- [Documentation](https://integration.growthzone.com)
- [Plans](plans/growthzone-plans-pricing.yml)
- [Rate Limits](rate-limits/growthzone-rate-limits.yml)
- [Fin Ops](finops/growthzone-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
