# Cloudflare D1

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

Cloudflare D1 is a managed, serverless SQLite database service with a REST API for querying D1 databases, executing SQL statements, listing databases, and managing database instances at the edge. D1 offers SQLite semantics, built-in Time Travel point-in-time recovery, global read replication, and seamless integration with Cloudflare Workers and Pages.

## Links

- **Website**: https://www.cloudflare.com/developer-platform/d1/
- **Documentation**: https://developers.cloudflare.com/d1/
- **API Reference**: https://developers.cloudflare.com/api/resources/d1/
- **Pricing**: https://developers.cloudflare.com/d1/platform/pricing/
- **Limits**: https://developers.cloudflare.com/d1/platform/limits/
- **Status**: https://www.cloudflarestatus.com/
- **Blog**: https://blog.cloudflare.com/
- **GitHub**: https://github.com/cloudflare
- **TypeScript SDK**: https://github.com/cloudflare/cloudflare-typescript
- **Release Notes**: https://developers.cloudflare.com/d1/platform/release-notes/

## APIs

- **Cloudflare D1 API** — REST API for managing and querying D1 serverless SQLite databases. Base URL: `https://api.cloudflare.com/client/v4`

### Key Endpoints

| Method | Path | Description |
|--------|------|-------------|
| GET | `/accounts/{account_id}/d1/database` | List all D1 databases |
| POST | `/accounts/{account_id}/d1/database` | Create a new D1 database |
| GET | `/accounts/{account_id}/d1/database/{database_id}` | Get a specific database |
| DELETE | `/accounts/{account_id}/d1/database/{database_id}` | Delete a database |
| POST | `/accounts/{account_id}/d1/database/{database_id}/query` | Execute SQL query (returns objects) |
| POST | `/accounts/{account_id}/d1/database/{database_id}/raw` | Execute SQL query (returns arrays) |
| POST | `/accounts/{account_id}/d1/database/{database_id}/export` | Export database as SQL |
| POST | `/accounts/{account_id}/d1/database/{database_id}/import` | Import SQL into database |
| GET | `/accounts/{account_id}/d1/database/{database_id}/time_travel/bookmark` | Get Time Travel bookmark |
| POST | `/accounts/{account_id}/d1/database/{database_id}/time_travel/restore` | Restore to point in time |

## Files

- `apis.yml` — APIs.json 0.19 index for this provider
- `plans/cloudflare-d1-plans-pricing.yml` — API Commons Plans 0.1 pricing details
- `rate-limits/cloudflare-d1-rate-limits.yml` — API Commons Rate Limits 0.1
- `finops/cloudflare-d1-finops.yml` — FinOps Framework 1.0 FOCUS-aligned cost management
