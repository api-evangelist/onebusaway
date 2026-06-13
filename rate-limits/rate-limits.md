# OneBusAway API Rate Limits

## Overview

OneBusAway is an open-source platform; there are no globally published, fixed
rate limits for all deployments. Each OneBusAway server instance independently
controls throttling on a per-API-key basis. The information below describes
the rate-limiting architecture and what developers should expect when
integrating against any OneBusAway deployment, including the public Puget
Sound reference server at `https://api.pugetsound.onebusaway.org`.

**Official configuration documentation:**
https://developer.onebusaway.org/guides/api-webapp-configuration-guide

## Authentication and Key-Based Throttling

All API requests require an `apiKey` passed as the `key` query parameter:

```
GET /api/where/arrivals-and-departures-for-stop/{stopID}.json?key=YOUR_KEY
```

API keys are issued by each deployment's administrator. Through the admin
interface (`/admin/api-keys.action`) or via `data-sources.xml`, administrators
configure per-key traffic allowances. The platform describes this as "a loose
form of authentication" used for access control and usage tracking.

## Connection Throttling

OneBusAway "supports basic connection throttling to prevent a single client
from abusing the API service." Throttle limits are set per API key and per
deployment. Specific numeric thresholds are not publicly disclosed; contact
the operator of the deployment you are targeting for limits that apply to
your key.

## HTTP Status Codes

| Code | Meaning |
|------|---------|
| 200 | Success |
| 400 | Bad request (invalid parameters) |
| 401 | Unauthorized (invalid or missing API key) |
| 404 | Resource not found |
| 429 | Rate limit exceeded — back off and retry |
| 500 | Server error |

## SDK Retry Behavior

Official SDKs (JavaScript, Python, Go, Java, Kotlin, Ruby) automatically retry
HTTP 429 responses with exponential backoff. Default retry count is 2. This
behavior is configurable at SDK initialization.

## Response Formats

- Append `.json` to endpoint paths for JSON responses.
- Append `.xml` for XML responses.
- JSON responses accept an optional `callback` query parameter for JSONP
  (cross-origin browser access).

## Timestamps

- All timestamps are milliseconds since Unix epoch, or human-friendly format:
  `yyyy-MM-dd_HH-mm-ss`.

## Best Practices

1. Cache responses where transit data changes infrequently (agency, route, stop
   details).
2. Use arrivals-and-departures endpoints only as frequently as needed for your
   UI refresh rate — real-time data typically changes every 15–30 seconds.
3. Implement exponential backoff with jitter on HTTP 429 responses.
4. Reuse your API key across requests; do not generate a new key per session.
5. For high-volume or production use, contact the deployment operator to
   discuss appropriate key quotas or consider self-hosting.

## Puget Sound Reference Deployment

The publicly accessible Puget Sound server (`api.pugetsound.onebusaway.org`)
is operated as a community resource. Be a good citizen: avoid polling at
intervals faster than your application genuinely requires, and do not scrape
the full dataset in bulk without coordination with the operator.

## Self-Hosted Deployments

Organizations running their own OneBusAway instance configure rate limits
through the admin UI or `data-sources.xml`. The `CreateApiKeyAction` bean
allows automatic key provisioning on startup with configurable traffic
allowances per key.
