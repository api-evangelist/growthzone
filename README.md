# GrowthZone (growthzone)

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
