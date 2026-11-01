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

13,072 original source frames passed native decoding and geometry save/restore checks. The library has 124 spatial/time shards, allowing the App to select available original frames for a viewport and astronomical year without a query server or user-generated files. Original Feature geometries, holes and source dates are preserved. The index and source files declare exact byte counts and SHA-256; clients still validate them before use.

This is a library of research sources, not complete global historical coverage. 725 original source frames are excluded by indexing, geometry or native compatibility checks. Native checks are not historical verification or approval of borders. Publication/rights/installation approval flags remain false; this library is not an approved installable public dataset. The earlier two regional collections remain available above.

Source: Seshat Cliopatria v0.2.1, Seshat Global History Databank (Ed Chalstrey, James Bennett), CC BY 4.0. See [world attribution](research/world/v1/ATTRIBUTION.md) and the root sourceLicense. Source rows were extracted unchanged into content-addressed files; spatial and temporal indexes were added. No border repairs, interpolation, or substitute years were introduced.
