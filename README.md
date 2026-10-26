# OneBusAway (onebusaway)

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
