# Enphase Energy (enphase-energy)

Enphase Energy (NASDAQ: ENPH) is a global home-energy technology company best known for pioneering microinverter-based solar — small grid-tied inverters that sit at each module rather than as a central string inverter — and for the Enlighten monitoring cloud that ties their fleet together. The product portfolio spans IQ Microinverters (IQ8/IQ9 family), IQ Battery storage, IQ EV Chargers, and the Enphase App (formerly Enlighten) for homeowners and installers.

The Enlighten Systems API exposes that monitoring fabric to third parties via an OAuth 2.0 protected JSON API at `api.enphaseenergy.com/api/v4` — covering systems search and inventory, energy and consumption time series, microinverter and meter telemetry, battery telemetry and settings, Storm Guard, grid status, load control, live data streaming, and IQ EV charger sessions. A companion **Commissioning API** serves qualifying installers (Partner plan) for activation, company, and user management.

**URL:** [Visit APIs.yml](https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

Solar, Energy, Microinverters, Battery Storage, IQ Battery, IQ Microinverter, IQ EV Charger, Enlighten, Home Energy Management, Renewable Energy, Grid Services, Cleantech, IoT, Telemetry, NASDAQ ENPH

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Enphase Enlighten Systems API v4 (Monitoring)

JSON-based, OAuth 2.0 protected v4 Monitoring API at `https://api.enphaseenergy.com/api/v4`. Exposes systems inventory, energy and consumption lifetime time series, revenue-grade meter readings, microinverter and meter telemetry, IQ Battery telemetry and settings, Storm Guard, grid status, load control, live data streaming, and IQ EV charger sessions. Access tokens valid 24 hours; refresh tokens 30 days. Every request additionally requires the per-application API key.

**Human URL:** [https://developer-v4.enphase.com/](https://developer-v4.enphase.com/)

- [Portal](https://developer-v4.enphase.com/)
- [Documentation](https://developer-v4.enphase.com/docs)
- [Quickstart](https://developer-v4.enphase.com/docs/quickstart.html)
- [OpenAPI](openapi/enphase-enlighten-v4-monitoring-openapi.yml)
- [Naftiko Capability — System Monitoring](capabilities/system-monitoring.yaml)
- [Naftiko Capability — Battery Management](capabilities/battery-management.yaml)
- [Naftiko Capability — EV Charging](capabilities/ev-charging.yaml)

### Enphase Enlighten Commissioning API

Installer-facing companion to the Monitoring API, available on the qualified Partner plan. Activation creation/update, company and user management, and tariff updates used to streamline Enlighten activation workflows from field tools.

**Human URL:** [https://developer-v4.enphase.com/](https://developer-v4.enphase.com/)

- [Portal](https://developer-v4.enphase.com/)
- [Documentation](https://developer-v4.enphase.com/docs)
- [Naftiko Capability — Commissioning](capabilities/commissioning.yaml)

### Enphase Enlighten Systems API v2 (Legacy)

The original v2 Enlighten Systems API. End-of-life was extended to June 30, 2024 and new applications should target v4. Retained in this catalog as a migration reference. Uses `key` + `user_id` query parameters rather than OAuth 2.0.

**Human URL:** [https://developer.enphase.com/docs](https://developer.enphase.com/docs)

- [Portal](https://developer.enphase.com/)
- [Documentation](https://developer.enphase.com/docs)
- [OpenAPI](openapi/enphase-enlighten-v2-openapi.yml)

## Plans

| Plan | Price | Per-Minute Limit | Monthly Quota | Overage | Notes |
|---|---|---|---|---|---|
| Watt | Free | 10/min | 10,000 | n/a | Attribution required ("Powered by Enphase Energy"). |
| Kilowatt | $25/mo | 50/min | 25,000 | $0.002/call | Commercial use; attribution waived. |
| Megawatt | $250/mo | 100/min | 300,000 | $0.002/call | Includes streaming/live data endpoints. |
| Gigawatt | $1,500/mo | 300/min | 1,500,000 | $0.001/call | Uptime guarantee. |
| Partner | Contact | Contact | Contact | Contact | Commissioning API access for qualified installers (10+ installs). |

- [Plans (API Commons)](plans/enphase-energy-plans-pricing.yml)
- [Rate Limits (API Commons)](rate-limits/enphase-energy-rate-limits.yml)
- [FinOps (FOCUS)](finops/enphase-energy-finops.yml)

## Common Properties

- [Portal](https://enphase.com/)
- [Developer Portal](https://developer-v4.enphase.com/)
- [GitHub Organization](https://github.com/enphase)
- [Support](https://support.enphase.com/)
- [The Enlighten API — Support article](https://support.enphase.com/s/article/The-Enlighten-API)
- [Email — api@enphaseenergy.com](mailto:api@enphaseenergy.com)
- [API License Agreement](https://www.enphase.com/en-us/legal/api-license-agreement)
- [Privacy Policy](https://enphase.com/legal/privacy-policy)
- [Blog](https://enphase.com/blog)
- [Investor Relations](https://investor.enphase.com/)
- [LinkedIn](https://www.linkedin.com/company/enphase-energy)
- [Twitter](https://twitter.com/Enphase)
- [YouTube](https://www.youtube.com/user/enphaseenergy)

## Schemas, Vocabulary, and Rules

- [JSON Schema — System](json-schema/enphase-system-schema.json)
- [JSON Schema — Telemetry Interval](json-schema/enphase-telemetry-schema.json)
- [JSON Schema — Battery Settings](json-schema/enphase-battery-schema.json)
- [JSON Structure — System](json-structure/enphase-system-structure.json)
- [JSON-LD Context](json-ld/enphase-energy-context.jsonld)
- [Vocabulary](vocabulary/enphase-energy-vocabulary.yml)
- [Spectral Rules](rules/enphase-energy-rules.yml)

## Example Payloads

- [System Summary](examples/enphase-system-summary-example.json)
- [Production Meter Telemetry](examples/enphase-production-meter-telemetry-example.json)
- [Battery Settings](examples/enphase-battery-settings-example.json)

## Notes on the OpenAPI

The OpenAPI documents in this repo are sourced from publicly available community references that mirror Enphase's published Swagger:

- v4 paths reflect the [`andrewdmontgomery/Enphase-OpenAPI`](https://github.com/andrewdmontgomery/Enphase-OpenAPI) regeneration of Enphase's developer-v4 spec.
- v2 paths reflect the [`NathanBaulch/EnphaseOpenAPI`](https://github.com/NathanBaulch/EnphaseOpenAPI) regeneration of the legacy v2 spec.

Both are retained for archival and tooling purposes; for authoritative behavior consult [developer-v4.enphase.com](https://developer-v4.enphase.com/).
