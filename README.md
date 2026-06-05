# Enphase Energy (enphase-energy)

Enphase Energy (NASDAQ ENPH) is a global home-energy technology company best known for pioneering microinverter-based solar — small grid-tied inverters that sit at each module rather than as a central string inverter — and for the Enlighten monitoring cloud that ties their fleet together. The product portfolio spans IQ Microinverters (IQ8/IQ9 family), IQ Battery storage, IQ EV Chargers, and the Enphase App (formerly Enlighten) for homeowners and installers. The Enlighten Systems API exposes that monitoring fabric to third parties via an OAuth 2.0 protected JSON API at api.enphaseenergy.com/api/v4 — covering systems search and inventory, energy and consumption time series, microinverter and meter telemetry, battery telemetry and settings, Storm Guard, grid status, load control, live data streaming, and IQ EV charger sessions. A companion Commissioning API serves qualifying installers (Partner plan) for activation, company, and user management. The v2 Enlighten Systems API reached end-of-life on June 30, 2024 and is retained here for migration reference.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/apis.yml)

## Scope

- **Position:** Producing
- **Access:** 3rd-Party

## Tags

- Solar
- Energy
- Microinverters
- Battery Storage
- IQ Battery
- IQ Microinverter
- IQ EV Charger
- Enlighten
- Home Energy Management
- Renewable Energy
- Grid Services
- Cleantech
- IoT
- Telemetry
- NASDAQ ENPH

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### Enphase Enlighten Systems API v4 (Monitoring)

The Enlighten Systems API v4 (Monitoring API) is a JSON-based, OAuth 2.0 protected API that provides access to system-level, device-level, and battery-level performance data for Enphase photovoltaic and storage systems. It exposes systems search and inventory, energy and consumption lifetime time series, revenue-grade meter readings (RGM), microinverter and meter telemetry, IQ Battery telemetry and settings, Storm Guard, grid status, load control, live data streaming, and IQ EV charger session data. Access tokens are valid for 24 hours and refresh tokens for 30 days; all requests require an application API key in addition to the bearer token.

- **Human URL:** [https://developer-v4.enphase.com/](https://developer-v4.enphase.com/)
- **Base URL:** `https://api.enphaseenergy.com/api/v4`

#### Tags

- Solar
- Energy
- Microinverters
- Battery Storage
- IoT
- Monitoring
- Telemetry
- Time Series

#### Properties

- [Portal](https://developer-v4.enphase.com/)
- [Documentation](https://developer-v4.enphase.com/docs)
- [Getting Started](https://developer-v4.enphase.com/docs/quickstart.html)
- [Documentation](https://developer-v4.enphase.com/aboutproduct.html)
- [OpenAPI](openapi/enphase-enlighten-v4-monitoring-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/enphase-enlighten-v4-monitoring.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/enphase-enlighten-v4-monitoring.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [O Auth2](https://api.enphaseenergy.com/oauth/authorize)
- [O Auth2](https://api.enphaseenergy.com/oauth/token)

### Enphase Enlighten Commissioning API

The Commissioning API is the installer-facing companion to the Monitoring API. Available to Partner-plan customers (qualifying installers with 10+ installations), it allows activation creation and updates, company and user management, tariff and rate plan updates, and other administrative controls used to streamline Enlighten activation workflows from field tools. OAuth 2.0 authorization with the same authorize/token endpoints as the Monitoring API.

- **Human URL:** [https://developer-v4.enphase.com/](https://developer-v4.enphase.com/)
- **Base URL:** `https://api.enphaseenergy.com/api/v4`

#### Tags

- Solar
- Energy
- Commissioning
- Installer
- Activation
- Partner

#### Properties

- [Portal](https://developer-v4.enphase.com/)
- [Documentation](https://developer-v4.enphase.com/docs)
- [O Auth2](https://api.enphaseenergy.com/oauth/authorize)
- [O Auth2](https://api.enphaseenergy.com/oauth/token)
- [Postman Collection](collections/enphase-enlighten-v2.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/enphase-enlighten-v2.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/enphase-enlighten-v4-monitoring.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/enphase-enlighten-v4-monitoring.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Enphase Enlighten Systems API v2 (Legacy)

The original v2 Enlighten Systems API. End-of-life was extended to June 30, 2024 and new applications should target the v4 Monitoring API. Retained in this catalog as a historical reference for v2-to-v4 migration. Uses key + user_id query parameters rather than OAuth 2.0.

- **Human URL:** [https://developer.enphase.com/docs](https://developer.enphase.com/docs)
- **Base URL:** `https://api.enphaseenergy.com/api/v2`

#### Tags

- Solar
- Energy
- Microinverters
- Monitoring
- Legacy

#### Properties

- [Portal](https://developer.enphase.com/)
- [Documentation](https://developer.enphase.com/docs)
- [OpenAPI](openapi/enphase-enlighten-v2-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/enphase-enlighten-v2.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/enphase-enlighten-v2.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://enphase.com/)
- [Portal](https://developer-v4.enphase.com/)
- [Documentation](https://developer-v4.enphase.com/docs)
- [Documentation](https://developer.enphase.com/docs)
- [Getting Started](https://developer-v4.enphase.com/docs/quickstart.html)
- [Sign Up](https://developer-v4.enphase.com/admin/applications/new)
- [O Auth2](https://api.enphaseenergy.com/oauth/authorize)
- [O Auth2](https://api.enphaseenergy.com/oauth/token)
- [GitHub Organization](https://github.com/enphase)
- [Support](https://support.enphase.com/)
- [Support](https://support.enphase.com/s/article/The-Enlighten-API)
- [Email](api@enphaseenergy.com)
- [Terms of Service](https://www.enphase.com/en-us/legal/api-license-agreement)
- [Privacy Policy](https://enphase.com/legal/privacy-policy)
- [Blog](https://enphase.com/blog)
- [Press](https://investor.enphase.com/news-releases)
- [Investor Relations](https://investor.enphase.com/)
- [LinkedIn](https://www.linkedin.com/company/enphase-energy)
- [Twitter](https://twitter.com/Enphase)
- [YouTube](https://www.youtube.com/user/enphaseenergy)
- [Facebook](https://www.facebook.com/EnphaseEnergy)
- [Careers](https://enphase.com/careers)
- [Product Details](https://enphase.com/homeowners/microinverters)
- [Product Details](https://enphase.com/homeowners/storage)
- [Product Details](https://enphase.com/homeowners/ev-charger)
- [Product Details](https://enphase.com/homeowners/enphase-app)
- [Product Details](https://enphase.com/installers)
- [Plans](https://developer-v4.enphase.com/plans.html)
- [Plans](plans/enphase-energy-plans-pricing.yml)
- [Rate Limits](rate-limits/enphase-energy-rate-limits.yml)
- [Fin Ops](finops/enphase-energy-finops.yml)
- [Tool](https://github.com/NathanBaulch/EnphaseOpenAPI)
- [Tool](https://github.com/andrewdmontgomery/Enphase-OpenAPI)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
