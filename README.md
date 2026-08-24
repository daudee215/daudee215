<!-- Use this README in the special daudee215/daudee215 profile repository. -->

<p align="center">
  <img src="./assets/profile-banner.svg" alt="Daud Tasleem researcher at Polito GIS GeoAI BIM infrastructure and natural hazards banner" width="100%" />
</p>

<h1 align="center">Daud Tasleem</h1>

<p align="center">
  Researcher at Politecnico di Torino (Polito). Semantic modelling of geodata, geo-analytical question answering, GeoAI, and infrastructure digital twins.
</p>

<p align="center">
  <a href="https://daudee.com">Website</a>
  |
  <a href="https://www.linkedin.com/in/daud-tasleem-73aa27131/">LinkedIn</a>
  |
  <a href="https://scholar.google.com/citations?user=pKgC0QwAAAAJ&hl=en">Google Scholar</a>
  |
  <a href="https://github.com/daudee215">GitHub</a>
</p>

<p align="center">
  Updated August 2026. The public repositories below are runnable and tested. Client and product work stays private.
</p>

## Profile

I build geospatial systems that make the analysis checkable. Recent work concentrates on
the semantics of geodata: giving attributes explicit types, deriving which workflows those
types actually admit, and measuring whether the answers produced are any use to the people
who asked the question.

Alongside that runs applied infrastructure work at Polito, where the same concern appears
as data pipelines, hazard context, and 3D review surfaces for real corridors and assets.

## Featured work

### Geo-analytical question answering

Three packages written to work together. Each is runnable from a clean checkout and each
has a test suite that runs in CI.

| Repository | What it does |
| --- | --- |
| [typed-workflow-layer](https://github.com/daudee215/typed-workflow-layer) | A typed intermediate layer between a geo-analytical question and the workflows that answer it. Core concept data types, exhaustive workflow synthesis to a depth bound, cost-based ranking, and refusals that name the repairing transformation. Standard library only. |
| [geo-annotation-kit](https://github.com/daudee215/geo-annotation-kit) | Semantic annotation of geodata attributes, with inter-annotator agreement measured on the axis it belongs on. Krippendorff ordinal alpha, disagreement analysis, and gold standards that refuse to break ties. |
| [geoqa-study-harness](https://github.com/daudee215/geoqa-study-harness) | Running a user study on a question answering system. Workflow comparison as trees, power analysis before recruiting, and no export until the data is safe to publish. |

A corpus annotated in `geo-annotation-kit` produces the typed sources `typed-workflow-layer`
consumes. The answers its workflows produce are then scored in `geoqa-study-harness`.

**Tech:** `Python` `GeoPandas` `pytest` `GitHub Actions`

### natech-guidance-qa

[natech-guidance-qa](https://github.com/daudee215/natech-guidance-qa) is retrieval-grounded
question answering over the European Commission Joint Research Centre technical guidance on
Natech risk management, with the retrieval measured rather than read. The underlying system
comes from Politecnico di Torino work in April 2026 and is kept unchanged in `original/`.
The corpus validation and retrieval evaluation were added later, and every module docstring
states which part is which, so the difference is checkable rather than asserted.

**Tech:** `Python` `pytest`

### ModelRAIL Pro

A full-stack rail infrastructure monitoring prototype built around the real Ceva-Ormea
corridor in Piemonte, Italy. Five-stage pipeline from ingest to publish, GIS and InSAR
fusion with live updates, UAV planning, point-cloud visualisation, role-based access, and
audit logging. Private repository, available on request.

**Tech:** `JavaScript` `Node.js` `Express` `SQLite` `Cesium` `Mapbox GL` `Leaflet` `Three.js`

## Focus areas

| Area | What that means in practice |
| --- | --- |
| Semantic modelling of geodata | Core concept data types, attribute annotation, agreement measurement, and gold standards |
| Geo-analytical question answering | Workflow synthesis under type constraints, cost-based ranking, provenance, and refusal with a named repair |
| Evaluation | User studies, inter-annotator agreement, retrieval evaluation, and sizing a study before recruiting |
| GeoAI and remote sensing | Spatial analysis, deep learning for mapping, point clouds, and corridor-scale products |
| Infrastructure and natural hazards | Landslide, flood, subsidence, climate, and exposure context; digital twins and inspection workflows |
| Geospatial interfaces | Spatial dashboards, map interaction, terrain-aware views, and 3D review |

## Selected stack

`Python` `GeoPandas` `Rasterio` `Shapely` `GDAL` `PostGIS` `QGIS` `pytest` `JavaScript` `Node.js` `Cesium` `Mapbox GL` `Leaflet` `GeoJSON`

## Connect

- Website: [daudee.com](https://daudee.com)
- Google Scholar: [publications](https://scholar.google.com/citations?user=pKgC0QwAAAAJ&hl=en)
- GitHub: [@daudee215](https://github.com/daudee215)