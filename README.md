# Terraevia research data

Public research-reading excerpts for Terraevia. No App source code, personal data, database, or private build logs are included.

## Available collections

- China and Asia: 100 BCE, 117 CE, 700 CE.
- Europe: 800 CE, 1200 CE, 1600 CE.

These are selected source frames, not complete historical coverage or approved borders. Europe 800/1200 omit 6/49 candidate frames respectively. The source's original temporal declarations and geometries are preserved. `publicationApproved`, `rightsApproved` and `appInstallationApproved` remain false in the research catalogs; these files are never formal approved public datasets in the App.

## Source and attribution

Seshat Cliopatria v0.2.1, Seshat Global History Databank (Ed Chalstrey, James Bennett), CC BY 4.0. Original source: https://github.com/Seshat-Global-History-Databank/cliopatria/tree/v0.2.1 . License: https://creativecommons.org/licenses/by/4.0/ . See ATTRIBUTION.txt and each catalog's sourceLicense. Modification notice: selected original source rows only; catalog metadata was added for reading and download integrity.

## App entry

https://raw.githubusercontent.com/YoYotouna/Terraevia-data/main/research/v1/research-regions.json

The App publisher maintains this directory. App users do not need to build or generate it. Root and per-region catalogs declare exact file sizes and SHA-256 digests; the App rechecks source bytes and historical frames before use. No GitHub credentials belong in the App. Future hosting can use maps.diyper.com with regenerated matching catalog URLs.


## Global static world library

[World index](https://raw.githubusercontent.com/YoYotouna/Terraevia-data/main/research/world/v1/world-index.json)

13,227 original source frames passed native decoding and geometry save/restore checks. The library has 124 spatial/time shards, allowing the App to select available original frames for a viewport and astronomical year without a query server or user-generated files. Original Feature geometries, holes and source dates are preserved. The index and source files declare exact byte counts and SHA-256; clients still validate them before use.

This is a library of research sources, not complete global historical coverage. 570 original source frames are excluded by indexing, geometry or native compatibility checks. Native checks are not historical verification or approval of borders. Publication/rights/installation approval flags remain false; this library is not an approved installable public dataset. The earlier two regional collections remain available above.

Source: Seshat Cliopatria v0.2.1, Seshat Global History Databank (Ed Chalstrey, James Bennett), CC BY 4.0. See [world attribution](research/world/v1/ATTRIBUTION.md) and the root sourceLicense. Source rows were extracted unchanged into content-addressed files; spatial and temporal indexes were added. No border repairs, interpolation, or substitute years were introduced.

2026-11-02 source compatibility update: 155 additional original frames (878–1555 CE) are available after aligning drawing-only zero-length-edge handling with the native reader. Source coordinates and dates remain unchanged. Previously published content-addressed files remain available for cached clients.

## Extended historical rings (world/v2)

[World v2 index](https://raw.githubusercontent.com/YoYotouna/Terraevia-data/main/research/world/v2/world-index.json)

13,256 original source frames passed native decoding and geometry save/restore checks, across 124 spatial/time shards. This version supports readonly historical rings up to 4,096 vertices and includes 29 additional original frames, including the Russian Empire in 1900. Personal drawing limits are unchanged. The v1 index and its content-addressed files remain available for earlier clients.

541 original frames remain excluded. A local test of 24 city viewports across 1900, 1950, 2000 and 2024 loaded reviewed sources in 95 of 96 cases; Moscow 1950 remains unsupported due to hole contact. This is a technical source-availability check, not verification of historical accuracy or global coverage. Original source coordinates and dates are unchanged; all approval flags remain false. Source and CC BY 4.0 attribution are declared in [v2 attribution](research/world/v2/ATTRIBUTION.md).

## Exact hole vertex contacts (world/v3)

[World v3 index](https://raw.githubusercontent.com/YoYotouna/Terraevia-data/main/research/world/v3/world-index.json)

13,382 original source frames passed native decoding and region save/restore checks, across 124 shards. This version includes 126 additional original frames (323 BCE–2024 CE) after supporting valid single shared-vertex hole contacts. Coordinates, holes and dates are unchanged. The 126 additional raw geometries also passed independent GEOS 3.13.1 validity checks. Contact cycles, crossings, shared edges, T-junctions and nested holes remain unsupported. v1 and v2 remain unchanged for earlier clients.

A local test loaded sources in all 96 city/year cases and found the exact original source in each of 126 added-source viewports, including Moscow 1950. These checks do not establish historical accuracy, global coverage, or device rendering performance. 415 original records remain excluded. All approval flags remain false. The original CC BY 4.0 attribution is retained in [v3 attribution](research/world/v3/ATTRIBUTION.md).

## Source coordinate precision (world/v4)

[World v4 index](https://raw.githubusercontent.com/YoYotouna/Terraevia-data/main/research/world/v4/world-index.json)

13,393 original source frames passed native decoding, independent source-coordinate comparison and region save/restore checks, across 124 shards. Eleven additional unchanged original frames became readable after correcting native decimal-number conversion and replacing a fixed edge-contact tolerance with a robust orientation test. All extracted frame bytes match the prior candidate; source coordinates, dates and properties were not edited. The drawn coordinates were checked against independent typed Double decoding, allowing only removal of the closing duplicate and adjacent zero-length edges.

A local test loaded all 233 viewports, including all 11 newly readable original identities; 10 of these new sample views previously had no reviewed source. The remaining 404 original records comprise 385 non-POLITY records, six source-year issues and 13 invalid geometries. v1, v2 and v3 remain unchanged for earlier clients. These technical checks do not prove historical accuracy, complete global coverage or device rendering performance. Approval flags remain false; original CC BY 4.0 attribution is retained in [v4 attribution](research/world/v4/ATTRIBUTION.md).

## Composite history index (maintainer preview)

[Composite research index](https://raw.githubusercontent.com/YoYotouna/Terraevia-data/main/research/world/v4/history-index.json) pins the existing v4 world index and a separate [boundary catalog](research/world/v4/boundary-index.json). New clients can read independently attributed research supplements through the same viewport/year and cache workflow.

The boundary catalog currently contains **zero** supplemental documents. No OHM candidate has been added; the 13,393-frame primary collection and its files remain unchanged. The App default continues to use world/v4/world-index.json. This preview establishes the public metadata path, not additional historical coverage or an approved dataset. Future supplements must retain original source identity, dates, attribution and display-derivation evidence; known conflicts remain on hold.

## Annual research snapshot supplement (history-v2)

[Preview composite index](https://raw.githubusercontent.com/YoYotouna/Terraevia-data/main/research/history-v2/history-index.json) combines the unchanged CC BY 4.0 world/v4 primary library with a separate GPL version 3 Historical Basemaps data collection. It is not yet the App default. Three extracted original Features (Mexico, Ottoman Empire and Arabia (Nejd)) are eligible for research reading in **1914 only**; a British Protectorate record remains HOLD and is not activated. World-scale reconstruction, not certified historical boundaries or complete country coverage. Historical accuracy remains NOT_VERIFIED; formal approval remains NOT_GRANTED.

The [GPL collection](research/history-v2/gpl-historical-basemaps/README.md) includes verbatim upstream GeoJSON, README, year index, full licence and pinned provenance, with unchanged original Features and dated wrapper modification notices. Source: André Ourednik and Historical Basemaps contributors, revision da7a4b735ecef70aebdc9c73e409d8a2500d50f3. All previously published v1–v4 data remain unchanged.
