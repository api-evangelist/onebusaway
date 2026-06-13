# OneBusAway (onebusaway)

OneBusAway is an open-source real-time transit information platform managed by the Open Transit Software Foundation. It provides transit riders with real-time arrival predictions, service alerts, and schedule data for buses, trains, and other transit modes. The platform exposes a RESTful API that lets developers access agency information, stop data, route details, trip information, real-time arrivals and departures, vehicle positions, and service alerts. Authentication uses an API key passed as a query parameter. The reference deployment runs at api.pugetsound.onebusaway.org; many transit agencies host their own OneBusAway instances using the same API contract. Official SDKs are published for Go, Java, Kotlin, JavaScript/Node.js, Python, and Ruby, all generated from a shared OpenAPI 3.0 specification in the sdk-config repository.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/onebusaway/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/onebusaway/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** Open

## Tags

- Transit
- Public Transit
- Real-Time
- Arrivals
- Departures
- Bus
- GTFS
- Open Source
- Stop Data
- Trip Planning
- Service Alerts
- Vehicle Positions
- Open Data

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## APIs

### OneBusAway REST API

RESTful web service providing real-time and scheduled transit data for agencies running the OneBusAway platform. Endpoints cover agencies with coverage, individual agency details, routes, stops, trips, real-time arrivals and departures, active vehicle positions, schedule information for stops and routes, shape/polyline data, block configuration, search for stops and routes by location or name, and user-submitted problem reports. Authentication is an API key supplied as the "key" query parameter. Responses are available in both JSON and XML; JSON responses support an optional JSONP callback parameter. The reference server is the Puget Sound deployment at api.pugetsound.onebusaway.org; transit agencies can self-host using the open-source application modules.

- **Human URL:** [https://developer.onebusaway.org/api/where](https://developer.onebusaway.org/api/where)
- **Base URL:** `https://api.pugetsound.onebusaway.org`

#### Tags

- Transit
- Real-Time
- Arrivals
- Departures
- Stops
- Routes
- Trips
- Agencies
- Vehicle Positions
- Service Alerts
- Schedule
- GTFS

#### Properties

- [Documentation](https://developer.onebusaway.org/api/where)
- [Documentation](https://developer.onebusaway.org/api/where/methods)
- [Documentation](https://developer.onebusaway.org/api/where/elements)
- [OpenAPI](https://raw.githubusercontent.com/OneBusAway/sdk-config/main/openapi.yml)
- [SDK](https://developer.onebusaway.org/api/sdk)
- [GitHub Repository](https://github.com/OneBusAway/sdk-config) — OpenAPI + SDK Config

## Common Properties

- [Website](https://opentransitsoftwarefoundation.org/onebusaway/)
- [Portal](https://developer.onebusaway.org/)
- [Documentation](https://developer.onebusaway.org/api/where)
- [Documentation](https://developer.onebusaway.org/api/where/methods)
- [Documentation](https://developer.onebusaway.org/api/where/elements)
- [Getting Started](https://developer.onebusaway.org/guides/api-webapp-configuration-guide)
- [SDK](https://developer.onebusaway.org/api/sdk)
- [GitHub Organization](https://github.com/OneBusAway)
- [GitHub Repository](https://github.com/OneBusAway/onebusaway-application-modules) — Core Application Modules (Java)
- [GitHub Repository](https://github.com/OneBusAway/maglev) — Maglev — Next-Gen OBA REST API Server (Go)
- [GitHub Repository](https://github.com/OneBusAway/sdk-config) — OpenAPI Specification and SDK Config
- [GitHub Repository](https://github.com/OneBusAway/js-sdk) — JavaScript / Node.js SDK
- [GitHub Repository](https://github.com/OneBusAway/python-sdk) — Python SDK
- [GitHub Repository](https://github.com/OneBusAway/go-sdk) — Go SDK
- [GitHub Repository](https://github.com/OneBusAway/java-sdk) — Java SDK
- [GitHub Repository](https://github.com/OneBusAway/kotlin-sdk) — Kotlin SDK
- [GitHub Repository](https://github.com/OneBusAway/ruby-sdk) — Ruby SDK
- [GitHub Repository](https://github.com/OneBusAway/onebusaway-android) — Android App
- [GitHub Repository](https://github.com/OneBusAway/onebusaway-ios) — iOS App
- [GitHub Repository](https://github.com/OneBusAway/wayfinder) — Wayfinder Web App (SvelteKit)
- [App Store](https://apps.apple.com/app/onebusaway/id329380089)
- [Play Store](https://play.google.com/store/apps/details?id=com.joulespersecond.seattlebusbot)
- [Privacy Policy](https://opentransitsoftwarefoundation.org/privacy-policy/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
