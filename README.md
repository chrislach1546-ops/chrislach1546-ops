## Chris Lach

I'm building **[Sip](https://github.com/chrislach1546-ops/sip-app)** — a social café-discovery app
for Los Angeles, where the community rates cafés by what they actually drank, and you follow the
people whose taste you trust. Solo project, in App Store submission prep.

React Native / Expo · TypeScript · Supabase Postgres · ~3,000 real LA cafés built from
OpenStreetMap and Overture Maps.

**What I've been working on lately**

- **[sip-app](https://github.com/chrislach1546-ops/sip-app)** — architecture and engineering write-ups for
  the app. How a substring bug put steakhouses on a café map, why row-level security gets tested
  like application code, and how to merge two geodata sources without ever detaching a photo from
  the place it was taken.
- **[open-place-toolkit](https://github.com/chrislach1546-ops/open-place-toolkit)** — nine
  dependency-free Node modules extracted from Sip's data pipeline. OSM `opening_hours` parsing,
  schema.org hours extraction, spatially-indexed place matching, polygon city resolution, and a
  robots.txt-respecting fetcher. 137 tests, no dependencies.

**How I like to work**

Tests before logic. Security enforced in the database rather than the UI. Every data change
reviewable and reversible. When a rule looks correct but I can't prove what it decided, I go and
measure it — that's how I found 224 real cafés a distance-only matching rule had been silently
discarding.
