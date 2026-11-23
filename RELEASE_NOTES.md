## Czechia API endpoints, snapshot 16 Nov 2026

- 6,362 endpoints passed a keyless data call, tested 16 Nov 2026 (IST)
- 188 services · country CZ · 6,362 keyless JSON rows

### Download

- `Czechia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz`: the full list, 6,362 rows, 125.8 kB gzipped (2.0 MB as CSV), SHA-256 `1f7ed96b4e3450584c5333fe9892d4ef7a6a49f3ae1f0602e6d35b60f7aa1e5a`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Czechia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Czechia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 6,362 · Wrap one layer query as a get_layer_features tool: pass a where clause or a bounding box, return the matching features with a timeout.
- 📱 App features: 6,362 · Add the layers to an app map: read the layer once for its fields, then ask for the features in the visible area.
- 🧠 Grounding and data pipelines: 83 · Load the tables and layers on a schedule into your own store, so an agent can cite a dated source.
- 🧪 Evals and testing: 6,362 · Run your tool calls against a fixed set of URLs across formats and record which answer; last_tested is the baseline for your own re-tests.

### Changes

- First release
- Left out: 44 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 1 layer marked editable in the title (it can hold entries that people added).
- Left out: 1 police traffic-stop layer (it can hold details of people stopped).
- Left out: 5 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 44 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 2 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 1 row that is another address of an ArcGIS layer dropped for what it holds (one of the reasons above, found under another address of the layer).
- Left out: 84 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 8,022 rows of university, college and school organisations and hosts (many of their layers are students' work).
- Left out: 4 rows whose address is already in an earlier pack of the collection.
- Left out: 1,837 rows that are another address form of an ArcGIS layer already in an earlier pack of the collection (the same rows under another query).
- Left out: 2,950 rows that are a second address form of an ArcGIS layer in this list (the same rows under another query); one address is kept per layer, the newest test first.
- Overlap: 391 of these URLs are also in 59k-europe-region-arcgis-apis-for-agents.
- Overlap: 62 of these URLs are also in 25k-arcgis-server-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 16 Nov 2026; snapshot 16 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 16 Nov 2026.

Credit: Czechia API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 16 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
