## Chris Lach

I'm building **[Sip](https://github.com/chrislach1546-ops/sip-app)**, a social café-discovery app
for Los Angeles where the community rates cafés by what they actually drank, and you follow the
people whose taste you trust. It's a solo project, built from scratch since July 2026.
**Version 1.0 is in App Store review.**

React Native / Expo · TypeScript · Supabase Postgres · 2,600 real LA cafés built from
OpenStreetMap and Overture Maps and checked against their current listings.

<p>
  <a href="https://github.com/chrislach1546-ops/sip-app"><img src="https://raw.githubusercontent.com/chrislach1546-ops/sip-app/main/screenshots/1-map.jpg" width="140" alt="Sip's map of LA cafés"></a>
  <a href="https://github.com/chrislach1546-ops/sip-app"><img src="https://raw.githubusercontent.com/chrislach1546-ops/sip-app/main/screenshots/3-cafe-detail.jpg" width="140" alt="A café page, rated by real visits"></a>
  <a href="https://github.com/chrislach1546-ops/sip-app"><img src="https://raw.githubusercontent.com/chrislach1546-ops/sip-app/main/screenshots/4-sip-viewer.jpg" width="140" alt="A single sip: one drink, one photo, one rating"></a>
  <a href="https://github.com/chrislach1546-ops/sip-app"><img src="https://raw.githubusercontent.com/chrislach1546-ops/sip-app/main/screenshots/5-profile.jpg" width="140" alt="A profile with badges earned from what you drink"></a>
</p>

**What I've been working on lately**

- **[sip-app](https://github.com/chrislach1546-ops/sip-app)**: the app's status, screenshots, and
  architecture and engineering write-ups. How a substring bug put steakhouses on a café map, why
  row-level security gets tested like application code (2,241 database assertions, run on every
  push), and how to merge two geodata sources without ever detaching a photo from the place it was
  taken.
- **[open-place-toolkit](https://github.com/chrislach1546-ops/open-place-toolkit)**: nine
  dependency-free Node modules from Sip's data pipeline. OSM `opening_hours` parsing,
  schema.org hours extraction, spatially-indexed place matching, polygon city resolution, and a
  robots.txt-respecting fetcher. 137 tests, no dependencies.

**How I like to work**

Tests before logic. Security enforced in the database rather than the UI. Every data change
reviewable and reversible. When a rule looks correct but I can't prove what it decided, I go and
measure it. That's how I found 224 real cafés a distance-only matching rule had been silently
discarding.
