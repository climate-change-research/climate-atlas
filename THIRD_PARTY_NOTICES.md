# Climate Atlas greenery Stage 1 third-party notices

Project ID: WEB-GREENERY-001  
Notice date: 2026-08-24

## Project license boundary

Copyright © 2026 John Luikart. All rights reserved. No open-source or
open-content license is granted for project-authored code, text, design, data
compilations, or branding unless a file expressly states otherwise.

Third-party software and data retain their own terms. The public deployment is
limited to the checksum-locked allowlist documented by this repository; it does
not publish private research history or complete original source archives.

## Bundled data and display assets

### MODIS MCD12Q1 Collection 6.1

- Use: 2024 terrestrial cover, cropland, and permanent-wetland display layers;
  the cover layer includes sparse/barren and snow/ice context, and natural
  versus managed status is unresolved.
- Publisher: NASA EOSDIS LP DAAC.
- Identifier: MCD12Q1.061.A2024001.
- Source resolution: 500 m.
- Source-product release: 5 August 2022.
- Selected-asset production/update: 30 July 2025.
- Citation: Friedl and Sulla-Menashe, MCD12Q1 Version 6.1.
- Terms: NASA EOSDIS Data Use and Citation Guidance; openly shared under the
  applicable NASA data policy, with citation requested.
- Record:
  https://doi.org/10.5067/MODIS/MCD12Q1.061

### MODIS MOD13A3 Collection 6.1

- Use: July 2026 NDVI greenness display.
- Publisher: NASA EOSDIS LP DAAC.
- Identifier: MOD13A3.061.A2026182.
- Source-product release: 16 February 2021.
- Current LPCLOUD inventory maximum metadata-update date: 17 August 2026. GIBS
  maps the legacy LPDAAC_ECS v061 concept, so this is not proven to be the GIBS
  tile-render update date.
- Citation: Didan, MOD13A3 Version 6.1.
- Terms: NASA EOSDIS Data Use and Citation Guidance; openly shared under the
  applicable NASA data policy, with citation requested.
- Record:
  https://doi.org/10.5067/MODIS/MOD13A3.061

### Global Lakes and Wetlands Database v2.0

- Use: broad wetland-type context derived from heterogeneous inputs spanning
  approximately 1990–2020.
- Publisher: HydroSHEDS and McGill University.
- Identifier: GLWD.2.0.MAIN_CLASS.
- Source-product and selected-asset date: 23 May 2025.
- Attribution: Lehner et al. (2025), Global Lakes and Wetlands Database v2.0;
  HydroSHEDS and McGill University.
- License: Creative Commons Attribution 4.0 International.
- Record:
  https://doi.org/10.6084/m9.figshare.28519994
- License:
  https://creativecommons.org/licenses/by/4.0/

The publisher additionally requests that the complete original-format dataset
not be mirrored elsewhere without permission. The website bundles only a small
transformed display image. An exact original-format copy is retained strictly
in the private owner-controlled GitHub/Drive preservation set, not authorized
for public redistribution; a public mirror remains blocked without written
permission.

### NASA GIBS PACE/OCI chlorophyll-a

- Use: provisional, incomplete 20 August 2026 daily chlorophyll-a proxy
  quick-look.
- Publisher: NASA Global Imagery Browse Services, with imagery supplied by the
  NASA Ocean Biology Processing Group.
- Identifier: GIBS.OCI_PACE_Chlorophyll_a.2026-08-20.
- Official GIBS layer-metadata publication/release date: not stated in the
  preserved response body. An HTTP update header was observed during audit but
  is not promoted into a source-product release date.
- Tile and mapping-response retrieval/freeze date: 22 August 2026. The
  upstream release, production, and update dates are not established.
- Attribution: NASA PACE Project and NASA Ocean Biology Processing Group.
- Terms: NASA EOSDIS Data Use and Citation Guidance; citation requested.
- GIBS record:
  https://gibs.earthdata.nasa.gov/layer-metadata/v1.0/OCI_PACE_Chlorophyll_a.json

The audited GIBS record lists PACE BGC source mappings only through NRT v3.1.
The separate 147-granule v3.2 CMR inventory for the same day is preserved as
context, not asserted as the provenance of the displayed tiles. Its 10
December 2024 value is identified only as a CMR metadata update date, not an
independently established v3.2 product release date.

### Global Mangrove Watch

- Use: 2025 mangrove-extent display.
- Version: 4.1.12.
- Source-product and selected-asset date: 13 July 2026.
- Attribution: © Global Mangrove Watch; Bunting et al. (2026), Global Mangrove
  Watch v4.1.12.
- License: Creative Commons Attribution 4.0 International.
- Record:
  https://doi.org/10.5281/zenodo.21346457
- License:
  https://creativecommons.org/licenses/by/4.0/

The displayed global raster includes a repository-added visibility halo. That
symbolization is disclosed and cannot be interpreted as source area.

### SeagrassSpotter through OBIS

- Use: a deterministic 500-point cartographic sample from 7,247 filtered,
  photo-associated direct seagrass occurrences with feature dates from
  2021–2025.
- Publisher: Project Seagrass via DASSH and the Ocean Biodiversity Information
  System.
- Identifier: OBIS.872b3454-7114-4ca9-914b-99b2518f86ee.
- Source-product and selected-asset date: 11 December 2025.
- Attribution: Unsworth, Jones, Rogers, Cullen-Unsworth and Lilley (2025),
  SeagrassSpotter; Project Seagrass, DASSH and OBIS.
- License: Creative Commons Attribution 4.0 International, as stated by the
  DASSH Integrated Publishing Toolkit and reverified 24 August 2026.
- Publisher record:
  https://www.dassh.ac.uk/ipt/resource?r=seagrassspotter
- License:
  https://creativecommons.org/licenses/by/4.0/

The points are occurrence evidence, not meadow geometry, absence, extent,
condition, permanence, trend, or representative global coverage. Attribution
and original evidence links remain with the derived point file.

### Natural Earth

- Use: generalized land polygons for cartographic context only.
- Version: Natural Earth 5.1.2, 1:110 million.
- Attribution: Made with Natural Earth.
- Terms: public domain.
- Record:
  https://github.com/nvkelso/natural-earth-vector/releases/tag/v5.1.2
- Terms:
  https://www.naturalearthdata.com/about/terms-of-use/

### Reported restoration initiatives

The point layer is a repository-authored factual compilation. Each feature
identifies its reporting authority, evidence URL, source-supported start-year
basis, and dated status or area evidence only when available. Unsupported dates
and areas remain null rather than being guessed. Conflicting official
terminology is preserved in qualifiers, and programme targets remain separate
from reported under-restoration or completed areas. No external project
geometry, logo, substantial source text, or claim of independent verification
is reproduced.

The compilation does not alter the rights in the linked authority records.
Copyright in the repository-authored selection and arrangement remains reserved
as described in `COPYRIGHT.md`.

## Software

The website directly uses MapLibre GL JS 6.5.0, distributed under the
BSD 3-Clause License:

https://github.com/maplibre/maplibre-gl-js/blob/v6.5.0/LICENSE.txt

Development and build dependencies include Vite, Vitest, TypeScript, and
GeoJSON type definitions. Their versions are pinned in
the private Development repository's package manifest, and each package retains its own license. The
scientific processing environment remains in the private Research repository.

The generated production dependency inventory is shipped under
`site/licenses/npm-production-licenses.json`, and the complete MapLibre
license text is shipped under `site/licenses/maplibre-gl-LICENSE.txt`.

## Deliberately unbundled candidates

Stage 1 does not redistribute:

- UNEP-WCMC global seagrass-extent geometry, because the audited terms restrict
  commercial use and redistribution;
- Allen Coral Atlas seagrass-extent geometry, pending a separate permissions
  review;
- Ramsar boundaries as vegetation extent;
- Copernicus Marine data pending a locked, credential-free, license-audited
  acquisition route;
- Global Pasture Watch cultivated-grassland probability v1, which was audited
  as a real peer-reviewed 2022 modelled or inferred source but requires an
  Earth Engine or substantially larger build-time ingestion decision.

The reasons and authoritative links are preserved in the
[source manifest](site/data/source-manifest.json).
