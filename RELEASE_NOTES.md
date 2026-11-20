## Air quality API endpoints, snapshot 15 Nov 2026

- 20,830 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 1,511 services · 247 country codes · 10,830 keyless JSON rows

### Download

- `Air_Quality_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 20,830 rows, 986.3 kB gzipped (7.2 MB as CSV), SHA-256 `8f64aadfb58ba85135aa4a7ba67732a6d7b2d555a4c63de8f521800d485854e8`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Air_Quality_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Air_Quality_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 8,148 · Wrap one URL pattern as a get_air_quality tool: pass a latitude and longitude or a station series id, return PM2.5, PM10, ozone and NO2 with the time of the reading.
- 📱 App features: 4,751 · Show PM2.5, PM10 and US AQI for a city on a card, and draw monitoring sites, pollution zones or modelled annual means as a map layer.
- 🧠 Grounding and data pipelines: 10,260 · Load station series and country PM2.5 figures on a schedule into your own store, so answers about air pollution cite a dated source.
- 🧪 Evals and testing: 20,830 · Run your air-quality tool against a fixed set of URLs across formats; check that pollutant, unit, value and timestamp parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release
- Left out: 158 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 1 layer marked editable in the title (it can hold entries that people added).
- Left out: 20 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 277 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 5 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Overlap: 20,830 of these URLs are also in 190k-weather-apis-for-agents.
- Overlap: 6,112 of these URLs are also in 270k-transit-apis-for-agents.
- Overlap: 400 of these URLs are also in 270k-water-apis-for-agents.
- Overlap: 16 of these URLs are also in 130k-finance-economy-apis-for-agents.
- Overlap: 12 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 365 of these URLs are also in 1.3m-government-open-data-apis.
- Overlap: 20 of these URLs are also in 290k-statistics-apis-for-agents.
- Overlap: 25 of these URLs are also in 86k-oceans-apis-for-agents.
- Overlap: 123 of these URLs are also in 24k-maritime-apis-for-agents.
- Overlap: 12,408 of these URLs are also in 170k-environment-apis-for-agents.
- Overlap: 560 of these URLs are also in 380k-maps-gis-apis-for-agents.
- Overlap: 10,830 of these URLs are also in 2.5m-agent-ready-apis.
- Overlap: 184 of these URLs are also in 96k-health-apis-for-agents.
- Overlap: 86 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 57 of these URLs are also in 53k-hazards-apis-for-agents.
- Overlap: 15 of these URLs are also in 6.5k-wildfire-apis-for-agents.
- Overlap: 117 of these URLs are also in 72k-energy-apis-for-agents.
- Overlap: 14 of these URLs are also in 25k-aviation-apis-for-agents.
- Overlap: 30 of these URLs are also in 24k-traffic-apis-for-agents.
- Overlap: 1 of these URLs is also in 12k-parking-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Air quality API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
