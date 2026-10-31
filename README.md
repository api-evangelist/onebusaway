# OneBusAway

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

**Areas:** Transit · Public Transit · Real-Time · Arrivals · Departures · Bus · GTFS · Open Source · Stop Data · Trip Planning · Service Alerts · Vehicle Positions

## OneBusAway on APIs.io

Everything profiled for OneBusAway is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/onebusaway/](https://apis.io/providers/onebusaway/)** — or go straight to one of the APIs or properties below.

### APIs (2)

- [OneBusAway Default API](https://apis.io/apis/onebusaway/onebusaway-default-api/) — The default API from OneBusAway — 13 operation(s) for default.
- [OneBusAway Where API](https://apis.io/apis/onebusaway/onebusaway-where-api/) — The Where API from OneBusAway — 17 operation(s) for where.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Onebusaway Agentic Access](https://apis.io/agentic-access/onebusaway/onebusaway-agentic-access/)

#### JSON Schema (61)

The data models the API reads and writes.

- [Agency](https://apis.io/schemas/onebusaway/Agency/)
- [AgencyResponse](https://apis.io/schemas/onebusaway/AgencyResponse/)
- [ArrivalDepartureForStop](https://apis.io/schemas/onebusaway/ArrivalDepartureForStop/)
- [ArrivalDepartureForStopResponse](https://apis.io/schemas/onebusaway/ArrivalDepartureForStopResponse/)
- [ArrivalsDeparturesForLocationResponse](https://apis.io/schemas/onebusaway/ArrivalsDeparturesForLocationResponse/)
- [ArrivalsDeparturesForStopResponse](https://apis.io/schemas/onebusaway/ArrivalsDeparturesForStopResponse/)
- [BlockConfiguration](https://apis.io/schemas/onebusaway/BlockConfiguration/)
- [BlockEntry](https://apis.io/schemas/onebusaway/BlockEntry/)
- [BlockResponse](https://apis.io/schemas/onebusaway/BlockResponse/)
- [BlockStopTime](https://apis.io/schemas/onebusaway/BlockStopTime/)
- [BlockTrip](https://apis.io/schemas/onebusaway/BlockTrip/)
- [Config](https://apis.io/schemas/onebusaway/Config/)
- [ConfigResponse](https://apis.io/schemas/onebusaway/ConfigResponse/)
- [Coverage](https://apis.io/schemas/onebusaway/Coverage/)
- [CoverageResponse](https://apis.io/schemas/onebusaway/CoverageResponse/)
- [CurrentTime](https://apis.io/schemas/onebusaway/CurrentTime/)
- [CurrentTimeResponse](https://apis.io/schemas/onebusaway/CurrentTimeResponse/)
- [DetailedScheduleStopTime](https://apis.io/schemas/onebusaway/DetailedScheduleStopTime/)
- [Location](https://apis.io/schemas/onebusaway/Location/)
- [Polylines](https://apis.io/schemas/onebusaway/Polylines/)
- [Reference](https://apis.io/schemas/onebusaway/Reference/)
- [ResponseWrapper](https://apis.io/schemas/onebusaway/ResponseWrapper/)
- [Route](https://apis.io/schemas/onebusaway/Route/)
- [RouteIDsForAgencyResponse](https://apis.io/schemas/onebusaway/RouteIDsForAgencyResponse/)
- [RouteResponse](https://apis.io/schemas/onebusaway/RouteResponse/)
- …and 36 more published on APIs.io

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [context Context](https://apis.io/jsonld/onebusaway/context/)

#### Examples (30)

Example requests and responses.

- [Getarrivalsanddeparturesforlocation](https://apis.io/examples/onebusaway/getArrivalsAndDeparturesForLocation/)
- [Get_Api_Where_Agencies With Coverage.Json](https://apis.io/examples/onebusaway/get_api_where_agencies-with-coverage.json/)
- [Get_Api_Where_Agency_Agencyid.Json](https://apis.io/examples/onebusaway/get_api_where_agency_agencyID.json/)
- [Get_Api_Where_Arrival And Departure For Stop_Stopid.Json](https://apis.io/examples/onebusaway/get_api_where_arrival-and-departure-for-stop_stopID.json/)
- [Get_Api_Where_Arrivals And Departures For Stop_Stopid.Json](https://apis.io/examples/onebusaway/get_api_where_arrivals-and-departures-for-stop_stopID.json/)
- [Get_Api_Where_Block_Blockid.Json](https://apis.io/examples/onebusaway/get_api_where_block_blockID.json/)
- [Get_Api_Where_Config.Json](https://apis.io/examples/onebusaway/get_api_where_config.json/)
- [Get_Api_Where_Current Time.Json](https://apis.io/examples/onebusaway/get_api_where_current-time.json/)
- [Get_Api_Where_Route Ids For Agency_Agencyid.Json](https://apis.io/examples/onebusaway/get_api_where_route-ids-for-agency_agencyID.json/)
- [Get_Api_Where_Route_Routeid.Json](https://apis.io/examples/onebusaway/get_api_where_route_routeID.json/)
- [Get_Api_Where_Routes For Agency_Agencyid.Json](https://apis.io/examples/onebusaway/get_api_where_routes-for-agency_agencyID.json/)
- [Get_Api_Where_Routes For Location.Json](https://apis.io/examples/onebusaway/get_api_where_routes-for-location.json/)
- [Get_Api_Where_Schedule For Route_Routeid.Json](https://apis.io/examples/onebusaway/get_api_where_schedule-for-route_routeID.json/)
- [Get_Api_Where_Schedule For Stop_Stopid.Json](https://apis.io/examples/onebusaway/get_api_where_schedule-for-stop_stopID.json/)
- [Get_Api_Where_Shape_Shapeid.Json](https://apis.io/examples/onebusaway/get_api_where_shape_shapeID.json/)
- [Get_Api_Where_Stop Ids For Agency_Agencyid.Json](https://apis.io/examples/onebusaway/get_api_where_stop-ids-for-agency_agencyID.json/)
- [Get_Api_Where_Stop_Stopid.Json](https://apis.io/examples/onebusaway/get_api_where_stop_stopID.json/)
- [Get_Api_Where_Stops For Agency_Agencyid.Json](https://apis.io/examples/onebusaway/get_api_where_stops-for-agency_agencyID.json/)
- [Get_Api_Where_Stops For Location.Json](https://apis.io/examples/onebusaway/get_api_where_stops-for-location.json/)
- [Get_Api_Where_Stops For Route_Routeid.Json](https://apis.io/examples/onebusaway/get_api_where_stops-for-route_routeID.json/)
- [Get_Api_Where_Trip Details_Tripid.Json](https://apis.io/examples/onebusaway/get_api_where_trip-details_tripID.json/)
- [Get_Api_Where_Trip For Vehicle_Vehicleid.Json](https://apis.io/examples/onebusaway/get_api_where_trip-for-vehicle_vehicleID.json/)
- [Get_Api_Where_Trip_Tripid.Json](https://apis.io/examples/onebusaway/get_api_where_trip_tripID.json/)
- [Get_Api_Where_Trips For Location.Json](https://apis.io/examples/onebusaway/get_api_where_trips-for-location.json/)
- [Get_Api_Where_Trips For Route_Routeid.Json](https://apis.io/examples/onebusaway/get_api_where_trips-for-route_routeID.json/)
- …and 5 more published on APIs.io

#### Collections (2)

Postman and Open Collection request collections.

- [OneBusAway default API](https://apis.io/collections/onebusaway/open-onebusaway-default-api/)
- [OneBusAway default Where API](https://apis.io/collections/onebusaway/open-onebusaway-where-api/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [OneBusAway — jsonschema rules](https://apis.io/rules/onebusaway/onebusaway-jsonschema-spectral-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Onebusaway Authentication](https://apis.io/security/onebusaway/onebusaway-authentication/)
- [Onebusaway Domain Security](https://apis.io/security/onebusaway/onebusaway-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Onebusaway Plans Pricing](https://apis.io/plans/onebusaway/onebusaway-plans-pricing/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://opentransitsoftwarefoundation.org/onebusaway/)
- [Documentation](https://developer.onebusaway.org/api/where)
- [Getting started](https://developer.onebusaway.org/guides/api-webapp-configuration-guide)
- [Blog](https://opentransitsoftwarefoundation.org/blog)
- [Privacy policy](https://opentransitsoftwarefoundation.org/privacy-policy/)
- [GitHub](https://github.com/OneBusAway)

## API Evangelist rating

**Kin Score 28.9** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 47.6 |
| Contract governance | 9.8 |
| Operational transparency | 2.6 |
| Developer ergonomics | 52.4 |
| Access clarity | 5.3 |

**Agent readiness 22.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 16.7** — Government & Public Sector

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/onebusaway/](https://apis.io/providers/onebusaway/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for OneBusAway: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/onebusaway/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
