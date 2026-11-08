# AGENTS.md – Repository Rules for AI Agents

## Context
This is a map-based volunteer directory for an Ottawa school club. The stack is [insert stack, e.g., Next.js + Leaflet].

## Key Files
- `/data/organizations.csv` – Master list of organizations.
- `/data/neighbourhoods.geojson` – Map boundaries (do not edit).
- `/src/components/Map` – Map component; uses Leaflet.

## Critical Rules
1. **Do not modify `geojson` files** unless explicitly instructed; they are sourced from Ottawa Open Data.
2. **Preserve the colour palette** defined in `tailwind.config.js` (garnet #8F001A, charcoal #2D2D2C, etc.).
3. **Admin routes** are under `/admin` and must be protected by authentication.
4. **Data integrity:** When adding organizations, validate against the CSV schema in `/data/README.md`.

## Workflows
- To add a new organization: update `organizations.csv` and run `npm run validate-data`.
- To regenerate the map: use the `scripts/fetch-geojson.js` utility.