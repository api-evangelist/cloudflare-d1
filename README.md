# Cloudflare D1

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
