# OneBusAway API FinOps

## Overview

OneBusAway is a fully open-source platform governed by the Open Transit
Software Foundation (OTSF), a volunteer-run nonprofit. There is no commercial
SaaS product with published API pricing. Cost exposure for teams integrating
OneBusAway falls into two buckets: consuming an existing public deployment
(near-zero cost) or operating a self-hosted deployment (infrastructure cost).

## Cost Structure

### Consuming a Public Deployment

Accessing any publicly hosted OneBusAway instance — such as the Puget Sound
reference server at `api.pugetsound.onebusaway.org` — is free. API keys are
issued at no charge by the deployment operator. There are no per-call fees,
monthly subscription fees, or overage charges.

**Cost to integrate:** $0 for API access; developer time only.

### Self-Hosting Costs

Organizations (transit agencies, municipalities, developers) can deploy
OneBusAway on their own infrastructure. Cost components include:

| Component | Notes |
|-----------|-------|
| Compute | JVM-based application modules (Java) or Maglev (Go); size depends on agency coverage and request volume |
| Storage | GTFS static data and realtime feeds; typically gigabytes not terabytes |
| GTFS-Realtime feed ingestion | May require connectivity to CAD/AVL hardware or a third-party feed |
| Docker / container orchestration | Docker images are available in the OneBusAway GitHub organization |
| TLS / domain | Required for production API hosting |

No licensing fees apply — OneBusAway is Apache 2.0 licensed.

### SDK and Tooling Costs

Official SDKs for JavaScript, Python, Go, Java, Kotlin, and Ruby are free and
open source. No per-seat or runtime licensing applies.

### Supporting the Open Transit Software Foundation

OTSF is donation-funded. Organizations that benefit from OneBusAway are
encouraged to contribute financially or through code. Donation information is
available at `https://opentransitsoftwarefoundation.org`.

## Cost Optimization Strategies

### For API Consumers

- **Cache static data** — agency, route, and stop details change infrequently;
  cache for hours or days rather than re-fetching per request.
- **Poll arrivals at reasonable intervals** — real-time arrival data updates
  every 15–30 seconds on most feeds; polling faster wastes bandwidth without
  improving accuracy.
- **Use location-based endpoints** — `stops-for-location`, `routes-for-location`,
  and `arrivals-and-departures-for-stop` return only relevant data, reducing
  payload size versus pulling full agency datasets.
- **JSONP only when necessary** — JSONP callbacks prevent browser caching;
  prefer CORS-compatible fetch patterns where possible.

### For Self-Hosted Deployments

- **Right-size compute** — start with the Docker deployment and measure actual
  CPU/memory before provisioning dedicated servers.
- **Use a CDN for static GTFS** — serving GTFS zip files through a CDN reduces
  origin load from third-party consumers.
- **Monitor per-key traffic** — the admin interface surfaces per-key usage;
  identify and throttle high-volume consumers before they affect other users.
- **Maglev for new deployments** — the Go-based Maglev server has a lower
  memory footprint than the Java application modules for agencies evaluating
  infrastructure costs.

## Financial Reporting Context

OneBusAway is deployed by dozens of transit agencies globally, including
agencies in the Puget Sound region, Tampa Bay, Washington DC metro area, and
internationally. Deployment and integration costs are absorbed by the operating
agencies as part of their IT budgets. No commercial entity controls or profits
from the open-source software itself.

## Contact

- **Open Transit Software Foundation:** https://opentransitsoftwarefoundation.org
- **Developer Documentation:** https://developer.onebusaway.org
- **GitHub Organization:** https://github.com/OneBusAway
- **Community Slack:** Available via the OTSF website for deployment support
