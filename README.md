<p align="center"><img src="assets/banner.svg" width="100%" alt="Czechia API endpoints: 6,362 API endpoints passed a keyless data call"></p>

# 🇨🇿 Czechia API endpoints

**6,362 API endpoints filed under country code CZ that answered a keyless GET with a data body. For agent and app builders.**

<p align="center"><a href="#files"><img src="https://img.shields.io/badge/endpoints-6%2C362-6366F1" alt="endpoints: 6,362"></a> <a href="#columns-and-tags"><img src="https://img.shields.io/badge/keyless%20JSON-6%2C362-6366F1" alt="keyless JSON: 6,362"></a> <a href="#whats-inside"><img src="https://img.shields.io/badge/services-188-0F172A" alt="services: 188"></a> <a href="#whats-inside"><img src="https://img.shields.io/badge/country-CZ-EA580C" alt="country: CZ"></a> <a href="LICENSE"><img src="https://img.shields.io/badge/licence-CC%20BY%204.0-0F172A" alt="licence: CC BY 4.0"></a></p>

<p align="center"><a href="#whats-in-it-for-you">What's in it</a> · <a href="#for-ai-agents">For AI agents</a> · <a href="#quick-start">Quick start</a> · <a href="#test-it-yourself">Test it yourself</a> · <a href="#files">Files</a> · <a href="#licence-and-credit">Licence</a> · <a href="#part-of-10m-api-endpoints-for-ai-agents">More packs</a></p>

This repository holds a 1,000-row sample and the services list; the full list of 6,362 endpoints is one download from the [latest release](https://github.com/agentpopulation/6.3k-czechia-apis-for-agents/releases/latest).

**Endpoints filed under country code CZ, for building an agent or app for Czechia.** Layers of Brno, the South Moravian Region and the national hydrometeorological institute, as URLs that answered with no key on their test date.

Selection rule: rows where `country is CZ`, less the rows that a leave-out rule drops (each counted under Known limits).

1,450 of these 6,362 rows match the focus rule (below); the others are in the pack by the selection rule only, and Known limits says what they are. 6,300 rows (99.0%) are map layers on ArcGIS Online, where anyone can publish.

## In plain words

**What is an API endpoint?** An API endpoint is one web address that a program can ask for data, for example the latest reading at one weather station. A single service, such as a national weather agency, can have thousands of endpoints: one per station, city or dataset. This pack counts endpoints, not separate services.

**What does "passed a data call" mean?** On the date shown in each row, AgentPopulation sent one plain request to that address, with no password or key, and got a non-empty data body back (JSON, CSV, XML or a file): not an error page and not an empty result. Some bodies describe a dataset rather than hold its values; see Known limits. It shows the address answered with data on that day. It is not a promise that it answers today, and licences and usage limits were not reviewed.

## What's in it for you

Four ways to use this pack. Each bucket gives a count, a filter you can apply to the CSV, one example that passed, and a list of recommended starting points with the rule that picked them. Buckets overlap; a row can fit more than one.

Examples, recommended lists and the preview are drawn from rows that match this pack's focus rule, so a row that the selection rule put in this pack but that is about something else is not shown as a starting point. Counts cover the whole bucket.

<details>
<summary>The focus rule</summary>

Focus rule: `NOT title matches /(?<![a-z])(test|tests|testing|draft|drafts|copy|sample|samples|demo|untitled|scratch|temp|tmp|delete|deleteme|practice|dummy|example|training)(?![a-z])|final_final|\d{7,}/i AND (NOT url matches ///(services[0-9]*(-[a-z0-9]+)?|utility)\.arcgis\.com//i OR NOT service matches /^ArcGIS organization /i)`

</details>

### 🤖 Agent tools: Keyless JSON layers and tables an agent can call (Czechia)

**6,362** endpoints from 188 services · Wrap one layer query as a get_layer_features tool: pass a where clause or a bounding box, return the matching features with a timeout.

6,362 of these are map-layer queries that asked for a few records (`resultRecordCount`); add a where clause or a geometry to ask about one place, and page through for the whole layer.

Start with: `tags has agent-ready`

Example: [1\_WFL1](https://services6.arcgis.com/fUWVlHWZNxUvTUh8/ArcGIS/rest/services/1_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) · Statutární město Brno (ArcGIS Online) · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and are tagged `agent-ready` (no key sent in the test call, JSON body, passed a data call). Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Sample preference in this bucket: `url matches //query\?/i`. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| Statutární město Brno (ArcGIS Online) (services6.arcgis.com) | 210 | 210 | CZ | json | [1\_WFL1](https://services6.arcgis.com/fUWVlHWZNxUvTUh8/ArcGIS/rest/services/1_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Jihomoravský kraj (ArcGIS Online) (services5.arcgis.com) | 150 | 150 | CZ | json | [Úspěšnost\_přijetí\_do\_mateřských\_škol\_v\_…](https://services5.arcgis.com/uc4BIJvwXwgPHm8D/ArcGIS/rest/services/%C3%9Asp%C4%9B%C5%A1nost_p%C5%99ijet%C3%AD_do_mate%C5%99sk%C3%BDch_%C5%A1kol_v_Jihomoravsk%C3%A9m_kraji_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Český hydrometeorologický ústav (ArcGIS Online) (services1.arcgis.com) | 128 | 128 | CZ | json | [1432\_ExpB\_WFL1](https://services1.arcgis.com/ZszVN9lBVA5x4VmX/ArcGIS/rest/services/1432_ExpB_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| 4ct s.r.o. (ArcGIS Online) (services5.arcgis.com) | 94 | 94 | CZ | json | [Brno\_Demolice\_budov\_ČD](https://services5.arcgis.com/YElTIrF9aD2PDrLy/ArcGIS/rest/services/Brno_Demolice_budov_%C4%8CD/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Pardubický kraj (ArcGIS Online) (services.arcgis.com) | 86 | 86 | CZ | json | [Železniční\_dráha](https://services.arcgis.com/S6UQzkU4EoJgYA53/ArcGIS/rest/services/%C5%BDelezni%C4%8Dn%C3%AD_dr%C3%A1ha/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| ArcGIS Demo portál (ArcGIS Online) (services.arcgis.com) | 70 | 70 | CZ | json | [A42vf](https://services.arcgis.com/qiROLxpdxrEizyHD/ArcGIS/rest/services/A42vf/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Výzkumný ústav vodohospodářský T.G.Masaryka, v.v.i. (ArcGIS Online) (services5.arcgis.com) | 52 | 52 | CZ | json | [ČOV2\_WFL1](https://services5.arcgis.com/o0IAVZMpUSHwNqMJ/ArcGIS/rest/services/%C4%8COV2_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Národní památkový ústav (ArcGIS Online) (services1.arcgis.com) | 50 | 50 | CZ | json | [325\_2004\_Sb](https://services1.arcgis.com/N9lESvcusHT2K1S7/ArcGIS/rest/services/325_2004_Sb/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 📱 App features: Map layers to draw in an app (Czechia)

**6,362** endpoints from 188 services · Add the layers to an app map: read the layer once for its fields, then ask for the features in the visible area.

Start with: `url matches //(Feature|Map)Server//i`

Example: [1\_WFL1](https://services6.arcgis.com/fUWVlHWZNxUvTUh8/ArcGIS/rest/services/1_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) · Statutární město Brno (ArcGIS Online) · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and passed a data call. Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| Statutární město Brno (ArcGIS Online) (services6.arcgis.com) | 210 | 210 | CZ | json | [1\_WFL1](https://services6.arcgis.com/fUWVlHWZNxUvTUh8/ArcGIS/rest/services/1_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Jihomoravský kraj (ArcGIS Online) (services5.arcgis.com) | 150 | 150 | CZ | json | [Úspěšnost\_přijetí\_do\_mateřských\_škol\_v\_…](https://services5.arcgis.com/uc4BIJvwXwgPHm8D/ArcGIS/rest/services/%C3%9Asp%C4%9B%C5%A1nost_p%C5%99ijet%C3%AD_do_mate%C5%99sk%C3%BDch_%C5%A1kol_v_Jihomoravsk%C3%A9m_kraji_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Český hydrometeorologický ústav (ArcGIS Online) (services1.arcgis.com) | 128 | 128 | CZ | json | [1432\_ExpB\_WFL1](https://services1.arcgis.com/ZszVN9lBVA5x4VmX/ArcGIS/rest/services/1432_ExpB_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| 4ct s.r.o. (ArcGIS Online) (services5.arcgis.com) | 94 | 94 | CZ | json | [Brno\_Demolice\_budov\_ČD](https://services5.arcgis.com/YElTIrF9aD2PDrLy/ArcGIS/rest/services/Brno_Demolice_budov_%C4%8CD/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Pardubický kraj (ArcGIS Online) (services.arcgis.com) | 86 | 86 | CZ | json | [Železniční\_dráha](https://services.arcgis.com/S6UQzkU4EoJgYA53/ArcGIS/rest/services/%C5%BDelezni%C4%8Dn%C3%AD_dr%C3%A1ha/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| ArcGIS Demo portál (ArcGIS Online) (services.arcgis.com) | 70 | 70 | CZ | json | [A42vf](https://services.arcgis.com/qiROLxpdxrEizyHD/ArcGIS/rest/services/A42vf/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Výzkumný ústav vodohospodářský T.G.Masaryka, v.v.i. (ArcGIS Online) (services5.arcgis.com) | 52 | 52 | CZ | json | [ČOV2\_WFL1](https://services5.arcgis.com/o0IAVZMpUSHwNqMJ/ArcGIS/rest/services/%C4%8COV2_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Národní památkový ústav (ArcGIS Online) (services1.arcgis.com) | 50 | 50 | CZ | json | [325\_2004\_Sb](https://services1.arcgis.com/N9lESvcusHT2K1S7/ArcGIS/rest/services/325_2004_Sb/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 🧠 Grounding and data pipelines: Statistics, boundaries, parcels and inventories for scheduled loads (Czechia)

**83** endpoints from 27 services · Load the tables and layers on a schedule into your own store, so an agent can cite a dated source.

Start with: `format in (csv, xml, geojson) OR title matches /statist|census|population|boundar|parcel|zoning|district|budget|election|crash|permit|inventory|land ?use|landuse|cadast|address/i`

Example: [Parcely\_WFL1](https://services5.arcgis.com/uc4BIJvwXwgPHm8D/ArcGIS/rest/services/Parcely_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) · Jihomoravský kraj (ArcGIS Online) · passed 2026-11-16

<details>
<summary>Recommended starting points: 7 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and passed a data call. Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| Jihomoravský kraj (ArcGIS Online) (services5.arcgis.com) | 3 | 150 | CZ | json | [Parcely\_WFL1](https://services5.arcgis.com/uc4BIJvwXwgPHm8D/ArcGIS/rest/services/Parcely_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| ARCDATA PRAHA, s.r.o. (ArcGIS Online) (services1.arcgis.com) | 2 | 30 | CZ | json | [covid19\_cze\_boundaries - kraje](https://services1.arcgis.com/gq83QRPZyW6Vjlnn/arcgis/rest/services/covid19_cze_boundaries/FeatureServer/1/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Kr Zlinsky (mapy.kr-zlinsky.cz) | 1 | 26 | CZ | json | [parcely](https://mapy.kr-zlinsky.cz/arcgis/rest/services/parcely/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Olomoucký kraj (ArcGIS Online) (services6.arcgis.com) | 1 | 20 | CZ | json | [budovy\_ok\_statistika](https://services6.arcgis.com/KPHdPhzFkBgzGlVf/ArcGIS/rest/services/budovy_ok_statistika/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Pardubický kraj (ArcGIS Online) (services.arcgis.com) | 1 | 86 | CZ | json | [PARCELY\_ClipCopy](https://services.arcgis.com/S6UQzkU4EoJgYA53/arcgis/rest/services/PARCELY_ClipCopy/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Urban Planner (ArcGIS Online) (services3.arcgis.com) | 1 | 26 | CZ | json | [parcely\_Znojmo](https://services3.arcgis.com/txiz4oPSebqpNQTJ/ArcGIS/rest/services/parcely_Znojmo/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| ZŠ Vápenná (ArcGIS Online) (services4.arcgis.com) | 1 | 8 | CZ | json | [worldPopulationProjection2100](https://services4.arcgis.com/qvM3dujM2P1ChTgX/ArcGIS/rest/services/worldPopulationProjection2100/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 🧪 Evals and testing: Varied responses to test tool calls and parsers

**6,362** endpoints · 188 services · country CZ · 1 format · Run your tool calls against a fixed set of URLs across formats and record which answer; last_tested is the baseline for your own re-tests.

Start with: the whole pack

Example: [1\_WFL1](https://services6.arcgis.com/fUWVlHWZNxUvTUh8/ArcGIS/rest/services/1_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) · Statutární město Brno (ArcGIS Online) · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack that returned the most different formats, then the most endpoints that passed a data call, then by name: a mix of response shapes to test parsers and tool calls. Here the services returned 1 format each, so the order comes down to endpoint counts. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| Statutární město Brno (ArcGIS Online) (services6.arcgis.com) | 210 | 210 | CZ | json | [1\_WFL1](https://services6.arcgis.com/fUWVlHWZNxUvTUh8/ArcGIS/rest/services/1_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Jihomoravský kraj (ArcGIS Online) (services5.arcgis.com) | 150 | 150 | CZ | json | [Úspěšnost\_přijetí\_do\_mateřských\_škol\_v\_…](https://services5.arcgis.com/uc4BIJvwXwgPHm8D/ArcGIS/rest/services/%C3%9Asp%C4%9B%C5%A1nost_p%C5%99ijet%C3%AD_do_mate%C5%99sk%C3%BDch_%C5%A1kol_v_Jihomoravsk%C3%A9m_kraji_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Český hydrometeorologický ústav (ArcGIS Online) (services1.arcgis.com) | 128 | 128 | CZ | json | [1432\_ExpB\_WFL1](https://services1.arcgis.com/ZszVN9lBVA5x4VmX/ArcGIS/rest/services/1432_ExpB_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| 4ct s.r.o. (ArcGIS Online) (services5.arcgis.com) | 94 | 94 | CZ | json | [Brno\_Demolice\_budov\_ČD](https://services5.arcgis.com/YElTIrF9aD2PDrLy/ArcGIS/rest/services/Brno_Demolice_budov_%C4%8CD/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Pardubický kraj (ArcGIS Online) (services.arcgis.com) | 86 | 86 | CZ | json | [Železniční\_dráha](https://services.arcgis.com/S6UQzkU4EoJgYA53/ArcGIS/rest/services/%C5%BDelezni%C4%8Dn%C3%AD_dr%C3%A1ha/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| ArcGIS Demo portál (ArcGIS Online) (services.arcgis.com) | 70 | 70 | CZ | json | [A42vf](https://services.arcgis.com/qiROLxpdxrEizyHD/ArcGIS/rest/services/A42vf/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Výzkumný ústav vodohospodářský T.G.Masaryka, v.v.i. (ArcGIS Online) (services5.arcgis.com) | 52 | 52 | CZ | json | [ČOV2\_WFL1](https://services5.arcgis.com/o0IAVZMpUSHwNqMJ/ArcGIS/rest/services/%C4%8COV2_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Národní památkový ústav (ArcGIS Online) (services1.arcgis.com) | 50 | 50 | CZ | json | [325\_2004\_Sb](https://services1.arcgis.com/N9lESvcusHT2K1S7/ArcGIS/rest/services/325_2004_Sb/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

The same lists are in [recommended.json](recommended.json), ready for an agent to load.

## Questions an agent can answer with this pack

- Which layers does the city of Brno publish? Try [1\_WFL1](https://services6.arcgis.com/fUWVlHWZNxUvTUh8/ArcGIS/rest/services/1_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (Statutární město Brno (ArcGIS Online), passed 2026-11-16).
- Which layers does the South Moravian Region publish? Try [Úspěšnost\_přijetí\_do\_mateřských\_škol\_v\_Jihomoravs…](https://services5.arcgis.com/uc4BIJvwXwgPHm8D/ArcGIS/rest/services/%C3%9Asp%C4%9B%C5%A1nost_p%C5%99ijet%C3%AD_do_mate%C5%99sk%C3%BDch_%C5%A1kol_v_Jihomoravsk%C3%A9m_kraji_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (Jihomoravský kraj (ArcGIS Online), passed 2026-11-16).
- Which layers does the Czech Hydrometeorological Institute publish? Try [1432\_ExpB\_WFL1](https://services1.arcgis.com/ZszVN9lBVA5x4VmX/ArcGIS/rest/services/1432_ExpB_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (Český hydrometeorologický ústav (ArcGIS Online), passed 2026-11-16).

## What "passed a data call" means

> [!NOTE]
> On the date in `last_tested` (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The `format` column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 16 Nov 2026; snapshot 16 Nov 2026.

## For AI agents

Start from keyless JSON endpoints (`agent-ready`). The code below loads `recommended.json` and calls the first recommended service in the Agent tools bucket, with a timeout (`node examples/agent-start.mjs --recommended`). With no argument, `node examples/agent-start.mjs` calls the most recently tested agent-ready row of the sample; pass a `.csv` or `.csv.gz` path to use that file instead. See [examples/agent-start.mjs](examples/agent-start.mjs).

```js
// Node 18+. Loads recommended.json (the local copy, or the raw file on GitHub) and calls one keyless JSON endpoint.
import fs from 'node:fs';

const RAW = 'https://raw.githubusercontent.com/agentpopulation/6.3k-czechia-apis-for-agents/main/recommended.json';
const rec = fs.existsSync('recommended.json')
  ? JSON.parse(fs.readFileSync('recommended.json', 'utf8'))
  : await (await fetch(RAW)).json();

const pick = rec.buckets.find((b) => b.id === 'agent').services[0];
try {
  const res = await fetch(pick.sample_url, {
    headers: { 'User-Agent': 'agent-example/1.0' },
    signal: AbortSignal.timeout(15000),
  });
  console.log(pick.service, res.status, res.headers.get('content-type'));
  console.log((await res.text()).slice(0, 300));
} catch (err) {
  console.log(`did not answer now; last passed ${pick.sample_last_tested} (${err.message})`);
}
```

How an agent picks an endpoint:

1. Filter to `agent-ready` and your country or topic.
2. Prefer the newest `last_tested` and the larger services.
3. Call with a timeout and check the body before you use it.

## Quick start

The examples run against the sample in `data/` out of the box (1,000 rows). Each takes an optional path to a `.csv` or `.csv.gz` file instead.

```bash
git clone https://github.com/agentpopulation/6.3k-czechia-apis-for-agents.git
cd 6.3k-czechia-apis-for-agents
python examples/quickstart.py
node examples/quickstart.mjs
node examples/agent-start.mjs
```

Full list: download `Czechia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz` (6,362 rows, 125.8 kB) from [releases/latest](https://github.com/agentpopulation/6.3k-czechia-apis-for-agents/releases/latest), then gunzip it and pass its path. The scripts also read the `.csv.gz` as it is.

```bash
gunzip Czechia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz
python examples/quickstart.py Czechia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv
node examples/quickstart.mjs Czechia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv
```

### curl

Quote the URL: some contain commas.

```bash
curl -sL "https://raw.githubusercontent.com/agentpopulation/6.3k-czechia-apis-for-agents/main/data/Czechia_API_Endpoints_AgentPopulation_Sample.csv" | head -n 4
curl -s --max-time 15 "https://services6.arcgis.com/fUWVlHWZNxUvTUh8/ArcGIS/rest/services/1_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json" | head -c 600
```

### Python

Standard library only: [examples/quickstart.py](examples/quickstart.py) reads the sample, or the path you pass, keeps agent-ready rows and calls the most recently tested one.

<details>
<summary>The code</summary>

```python
# Python 3, standard library only. Run from a clone of this repository:
#   python examples/quickstart.py [path]
# With no path it reads the sample in data/. Pass the full list from the latest release (.csv or .csv.gz) instead.
# Keeps agent-ready rows and calls the most recently tested one.
import csv
import gzip
import os
import re
import sys
import urllib.request

HERE = os.path.dirname(os.path.abspath(__file__))
path = sys.argv[1] if len(sys.argv) > 1 else os.path.join(HERE, "..", "data", "Czechia_API_Endpoints_AgentPopulation_Sample.csv")
opener = gzip.open if path.endswith(".gz") else open
with opener(path, "rt", newline="", encoding="utf-8") as f:
    rows = list(csv.DictReader(f))

agent = [r for r in rows if "agent-ready" in r["tags"].split("|")]
# Newest test date first; URLs that describe a dataset or a service rather than return values go last.
DESCRIBES = re.compile(r"/erddap/info/|action-report\.json$|[?&]request=getcapabilities|/GeoArea/[^/?]+/List|getFullTableDownloadCSV|hub\.worldpop\.org", re.I)
agent.sort(key=lambda r: r["last_tested"], reverse=True)
agent.sort(key=lambda r: 1 if DESCRIBES.search(r["url"]) else 0)
print(len(rows), "rows,", len(agent), "agent-ready")
if not agent:
    sys.exit(0)

row = agent[0]
req = urllib.request.Request(row["url"], headers={"User-Agent": "agent-example/1.0"})
try:
    with urllib.request.urlopen(req, timeout=15) as res:
        body = res.read(1_000_000).decode("utf-8", "replace")
        print(res.status, res.headers.get("Content-Type"))
        print(body[:300])
except Exception as err:
    print(f"did not answer now; last passed {row['last_tested']} ({err})")
```

</details>

### JavaScript

Reads the sample as JSON because the CSV has quoted commas.

<details>
<summary>The code</summary>

```js
// Node 18+. Reads the sample as JSON (the CSV has quoted commas), local file first.
import fs from 'node:fs';

const FILE = 'data/Czechia_API_Endpoints_AgentPopulation_Sample.json';
const rows = fs.existsSync(FILE)
  ? JSON.parse(fs.readFileSync(FILE, 'utf8'))
  : await (await fetch('https://raw.githubusercontent.com/agentpopulation/6.3k-czechia-apis-for-agents/main/data/Czechia_API_Endpoints_AgentPopulation_Sample.json')).json();

const row = rows.find((r) => r.tags.includes('agent-ready'));
const res = await fetch(row.url, { headers: { 'User-Agent': 'agent-example/1.0' }, signal: AbortSignal.timeout(15000) });
console.log(res.status, (await res.text()).slice(0, 300));
```

</details>

### Agent tools

[examples/agent-tools.json](examples/agent-tools.json) holds two tool definitions in the shape most tool-calling APIs accept (name, description, JSON Schema); rename `parameters` if yours uses another key. [examples/quickstart.mjs](examples/quickstart.mjs) implements them:

- `find_endpoints` searches the agent-ready rows of the list by words (their format is json). When you load the tools of more than one pack, prefix the names (for example `czechia_find_endpoints`) so they do not clash.
- `fetch_endpoint` calls one URL, **refuses any URL that is not in the list** and does not follow redirects. The allowlist is built from the CSV, so a URL injected into a prompt is refused.

The same two tools can sit behind an MCP server.

## Test it yourself

Re-test endpoints from the sample with the same rule: HTTP 2xx and a non-empty body that is not an HTML page. Node 18+, no packages.

```bash
node tools/test-endpoints.mjs
```

It tests the first 50 URLs and prints one line: tested, passed, did not pass. Options: a `.csv` or `.csv.gz` path (the full list from the release), `--limit 50`, `--timeout-ms 10000`, `--out results.csv`. The results file holds `url`, `status`, `passed`, `content_type`, `ms` and `checked_at`; a status of `timeout` or `error:<code>` means no HTTP answer came back. It is polite: GET only, no key sent, at most 4 requests in flight, one at a time per listed host, at least 1 second between requests to one listed host, and reading stops once 256 kB of a body is kept. Redirects are followed and may lead to another host. `results.csv` is in `.gitignore`.

## Preview

One row from each of the five largest services among rows that match the focus rule, services with rows that return values first.

| Title | Service | Country | Format | Tested | Link |
|---|---|---|---|---|---|
| 1\_WFL1 | Statutární město Brno (ArcGIS Online) | CZ | json | 2026-11-16 | [services6.arcgis.com](https://services6.arcgis.com/fUWVlHWZNxUvTUh8/ArcGIS/rest/services/1_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| Úspěšnost\_přijetí\_do\_mateřských\_škol\_v\_Jihomoravském\_kraji\_… | Jihomoravský kraj (ArcGIS Online) | CZ | json | 2026-11-16 | [services5.arcgis.com](https://services5.arcgis.com/uc4BIJvwXwgPHm8D/ArcGIS/rest/services/%C3%9Asp%C4%9B%C5%A1nost_p%C5%99ijet%C3%AD_do_mate%C5%99sk%C3%BDch_%C5%A1kol_v_Jihomoravsk%C3%A9m_kraji_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| Brno\_Demolice\_budov\_ČD | 4ct s.r.o. (ArcGIS Online) | CZ | json | 2026-11-16 | [services5.arcgis.com](https://services5.arcgis.com/YElTIrF9aD2PDrLy/ArcGIS/rest/services/Brno_Demolice_budov_%C4%8CD/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| 1432\_ExpB\_WFL1 | Český hydrometeorologický ústav (ArcGIS Online) | CZ | json | 2026-11-16 | [services1.arcgis.com](https://services1.arcgis.com/ZszVN9lBVA5x4VmX/ArcGIS/rest/services/1432_ExpB_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| Železniční\_dráha | Pardubický kraj (ArcGIS Online) | CZ | json | 2026-11-16 | [services.arcgis.com](https://services.arcgis.com/S6UQzkU4EoJgYA53/ArcGIS/rest/services/%C5%BDelezni%C4%8Dn%C3%AD_dr%C3%A1ha/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |

Browse the 1,000-row sample: [Sample CSV](data/Czechia_API_Endpoints_AgentPopulation_Sample.csv) · [Sample JSON](data/Czechia_API_Endpoints_AgentPopulation_Sample.json).

## What's inside

<p align="center"><img src="assets/breakdown.svg" width="100%" alt="Top categories and formats in this pack"></p>

<details>
<summary>Categories: top 8</summary>

| Category | Endpoints | |
|---|---:|---|
| Navigation & Geo/Maps | 3,266 | `████████████████████` |
| Government & Open Data | 2,589 | `███████████████▉` |
| Energy | 155 | `█` |
| Transport & Mobility | 117 | `▊` |
| Environment | 68 | `▍` |
| Statistics & Economy | 55 | `▍` |
| Health | 33 | `▎` |
| Maritime | 23 | `▏` |

</details>

Formats: json 6,362

<details>
<summary>Largest services: top 25 of 188</summary>

| Service | Host | Endpoints | Keyless JSON | |
|---|---|---:|---:|---|
| ArcGIS Online layers (services3.arcgis.com, org lOWgvXGCzs0MJj0p) † | services3.arcgis.com | 754 | 754 | `████████████████████` |
| ArcGIS Online layers (services2.arcgis.com, org kyjzwd0TLNHSVK1w) † | services2.arcgis.com | 751 | 751 | `███████████████████▉` |
| ArcGIS Online layers (services2.arcgis.com, org LlQJoYHf9cwrM7NJ) † | services2.arcgis.com | 583 | 583 | `███████████████▌` |
| ArcGIS Online layers (services.arcgis.com, org gn2pJn4aJIXiYlr9) † | services.arcgis.com | 357 | 357 | `█████████▌` |
| ArcGIS Online layers (services1.arcgis.com, org WJxRPR3k420mEqJx) † | services1.arcgis.com | 292 | 292 | `███████▊` |
| ArcGIS Online layers (services.arcgis.com, org ui1VEKalYDDIAi4N) † | services.arcgis.com | 281 | 281 | `███████▌` |
| Statutární město Brno (ArcGIS Online) | services6.arcgis.com | 210 | 210 | `█████▋` |
| ArcGIS Online layers (services7.arcgis.com, org 46Lck1orT7mvuzK5) † | services7.arcgis.com | 182 | 182 | `████▉` |
| ArcGIS Online layers (services7.arcgis.com, org A3ayBNlxwr6n2y8g) † | services7.arcgis.com | 168 | 168 | `████▌` |
| Jihomoravský kraj (ArcGIS Online) | services5.arcgis.com | 150 | 150 | `████` |
| ArcGIS Online layers (services6.arcgis.com, org MBLxaIHHJFo8VA1y) † | services6.arcgis.com | 136 | 136 | `███▋` |
| ArcGIS Online layers (services6.arcgis.com, org ogJAiK65nXL1mXAW) † | services6.arcgis.com | 130 | 130 | `███▌` |
| Český hydrometeorologický ústav (ArcGIS Online) | services1.arcgis.com | 128 | 128 | `███▍` |
| ArcGIS Online layers (services-eu1.arcgis.com, org RF0lYXxZ7gaXj7ZP) † | services-eu1.arcgis.com | 97 | 97 | `██▋` |
| 4ct s.r.o. (ArcGIS Online) | services5.arcgis.com | 94 | 94 | `██▌` |
| Pardubický kraj (ArcGIS Online) | services.arcgis.com | 86 | 86 | `██▎` |
| ArcGIS Online layers (services8.arcgis.com, org jfWD14yYevYeDEj7) † | services8.arcgis.com | 83 | 83 | `██▎` |
| ArcGIS Demo portál (ArcGIS Online) | services.arcgis.com | 70 | 70 | `█▉` |
| ArcGIS Online layers (services8.arcgis.com, org IyOEkZNvMiU8JI5H) † | services8.arcgis.com | 55 | 55 | `█▌` |
| Výzkumný ústav vodohospodářský T.G.Masaryka, v.v.i. (ArcGIS Online) | services5.arcgis.com | 52 | 52 | `█▍` |
| ArcGIS Online layers (services5.arcgis.com, org AAXTFOz7LQMwGEeO) † | services5.arcgis.com | 51 | 51 | `█▍` |
| Národní památkový ústav (ArcGIS Online) | services1.arcgis.com | 50 | 50 | `█▍` |
| Jihočeský kraj (ArcGIS Online) | services3.arcgis.com | 47 | 47 | `█▎` |
| ArcGIS Online layers (services6.arcgis.com, org 3K3x512LazHwGQL3) † | services6.arcgis.com | 45 | 45 | `█▎` |
| ArcGIS Online layers (services5.arcgis.com, org yoItBGzTbve2yig2) † | services5.arcgis.com | 44 | 44 | `█▏` |

† No row of these services matches the focus rule: the selection rule put them in this pack, so they are not used as a starting point.

</details>

<details>
<summary>Rows per test date: 16 Nov 2026</summary>

| Date (IST) | Endpoints | |
|---|---:|---|
| 2026-11-16 | 6,362 | `████████████████████` |

</details>

## Files

| File | Rows | Size | Use |
|---|---:|---:|---|
| [data/Czechia_API_Services_AgentPopulation.csv](data/Czechia_API_Services_AgentPopulation.csv) | 188 | 12.2 kB | One row per service with its endpoint count in this pack |
| [data/Czechia_API_Endpoints_AgentPopulation_Sample.csv](data/Czechia_API_Endpoints_AgentPopulation_Sample.csv) | 1,000 | 319.4 kB | The sample: focus-rule rows first, each service in proportion to its share; ArcGIS Online layers count as one service |
| [data/Czechia_API_Endpoints_AgentPopulation_Sample.json](data/Czechia_API_Endpoints_AgentPopulation_Sample.json) | 1,000 | 502.1 kB | The same rows as JSON, tags as an array |
| [Czechia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz](https://github.com/agentpopulation/6.3k-czechia-apis-for-agents/releases/latest) | 6,362 | 125.8 kB | The full list, gzipped CSV: a download from the latest release, checked by `SHA256SUMS.txt` |
| [tools/test-endpoints.mjs](tools/test-endpoints.mjs) | | | Re-tests endpoints from the sample or the full list |

Sample size: 1,000 rows, which is 1,000 or one third of the pack rounded down, whichever is smaller. Rows that match the focus rule come first. Each service gets rows in proportion to its share of those rows, at least one for the largest services and at most 50% of the sample while other services have rows; ArcGIS Online layers count as one service, whatever their organisation. Within a service, agent-ready rows, rows that return values and the newest test dates come first, and rows are written in turn across services. Service root addresses are placed at the end of the sample.

Full list: download `Czechia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz` (6,362 rows, 125.8 kB) from [releases/latest](https://github.com/agentpopulation/6.3k-czechia-apis-for-agents/releases/latest), then gunzip it and pass its path. The scripts also read the `.csv.gz` as it is.

Excel users: Data > From Text/CSV, UTF-8. Files are UTF-8 without a byte-order mark and comma-separated.

## Columns and tags

<details>
<summary>Columns, types and tags</summary>

| Column | Type | Example | Meaning |
|---|---|---|---|
| url | string | [https://services6.arcgis.com/fUWVlHWZNx…](https://services6.arcgis.com/fUWVlHWZNxUvTUh8/ArcGIS/rest/services/1_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) | The address that was tested |
| title | string | 1\_WFL1 | Station, dataset or feed name |
| service | string | Statutární město Brno (ArcGIS Online) | The service the endpoint belongs to; joins to the services file together with host |
| host | string | services6.arcgis.com | Host name of the address |
| country | string | CZ | ISO 3166-1 alpha-2 code, or EU; empty when global or unknown |
| category | string | Navigation & Geo/Maps | Category of the endpoint |
| subcategory | string |  | Left empty from the 15 Nov 2026 snapshot; kept so the columns stay the same |
| format | string | json | What the test call returned: json, csv, geojson, xml, gtfs, zip, txt and so on |
| tags | string | `no-key\|json\|agent-ready` | Tags separated by \| |
| last_tested | date | 2026-11-16 | Date of the test call, YYYY-MM-DD (IST) |

| Tag | Rows | Meaning |
|---|---:|---|
| agent-ready | 6,362 | No key sent, JSON body, passed a data call on last_tested |
| json | 6,362 | Format of the body |
| no-key | 6,362 | No key was sent in the test call |

A machine-readable copy of this dictionary is in [datapackage.json](datapackage.json).

</details>

## Known limits

- 6,362 rows are map-layer queries with resultRecordCount set: the tested call asked for a few records; change the query to get the full layer.
- 6,300 rows are layers on ArcGIS Online, where anyone can publish: some are class projects, tests or copies. Check the owner and the fields before you rely on one. Only layers of organisations with a name of their own, whose titles do not read as a test, draft or copy, are used as starting points.
- 218 rows have a title that reads as a test, a draft, a copy or a sample; they are not used as starting points.
- The country code (CZ) is the code the endpoint is filed under, not the place the data covers and not always the publisher's country. Where a row had no code, the code of its ArcGIS organisation is used when that organisation lists one country only. In a sample of 14 titles read before release, 1 was about a place outside Czechia. Filter by title or service if you need data about one place.
- Stations and feeds can go quiet after their test date; re-test a URL before you rely on it.
- Not in this pack: endpoints that need a key or a POST, and URLs that did not pass.
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

## Licence and credit

> [!IMPORTANT]
> This list (URLs, titles, tags and test results) is © 2026 AgentPopulation, released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit AgentPopulation and link agentpopulation.com. The data each endpoint returns belongs to its provider and stays under that provider's terms; this licence does not cover it.

Copy-ready credit:

`Czechia API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 16 Nov 2026.`

GitHub's "Cite this repository" button reads [CITATION.cff](CITATION.cff).

<!-- agentpopulation:start -->
## Part of 10M API endpoints for AI agents

This pack is one of the 50 topic packs of [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents), the open collection by [AgentPopulation](https://agentpopulation.com). Target: 10 million+ open API endpoints that pass a keyless API call.

AgentPopulation's test run of 16 Nov 2026: 4,452,803 tested, 3,346,053 passed a data call. This is the Czechia pack: 6,362 endpoints from 188 services, none of them in a pack read from the earlier snapshot, by address or as another address of the same map layer. Packs overlap, so an endpoint can appear in more than one.

For the latest tested endpoints, search [agentpopulation.com/apis](https://agentpopulation.com/apis). This pack is a snapshot from 16 Nov 2026.

Sibling packs that share the most URLs with this one: [59k-europe-region-arcgis-apis-for-agents](https://github.com/agentpopulation/59k-europe-region-arcgis-apis-for-agents) (391 shared) · [25k-arcgis-server-apis-for-agents](https://github.com/agentpopulation/25k-arcgis-server-apis-for-agents) (62 shared). The rest are listed in [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents).

Questions, pack requests, reports of endpoints that stopped answering and requests to remove a row go to [Discussions](https://github.com/agentpopulation/10m-open-apis-for-ai-agents/discussions), or to [@agentpopulation](https://x.com/agentpopulation) on X. The packs are a work in progress and corrections are welcome.

Spotted a wrong row or a dead URL? Tell us on X: [@agentpopulation](https://x.com/agentpopulation).

If this pack saved you time, a star helps others find it.

---

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents)

<!-- agentpopulation:end -->
