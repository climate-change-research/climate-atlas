# Climate Atlas

Public, static deployment of the Climate Atlas: scientifically explicit maps
of Earth's greenery, oceans, ice, temperature, and environmental change through
time.

The first module, **Earth's greenery**, is a low-resolution multi-source
reference snapshot. It is not a live or perfectly synchronized image. Every
layer keeps its actual observation window, evidence category, coverage,
resolution, source, rights, and limitations.

Expected GitHub Pages URL:
https://climate-change-research.github.io/climate-atlas/

## Repository boundary

This is a deployment-only repository. It contains the exact compiled static
site, public scientific provenance, checksums, copyright record, third-party
notices, and hosting workflows. It does not contain application source, tests,
private research history, raw scientific source archives, private custody
locators, credentials, or source maps.

- [`climate-change-research/Research`](https://github.com/climate-change-research/Research)
  is the private scientific backbone and complete source-data custodian.
- [`climate-change-research/Climate-Atlas-Development`](https://github.com/climate-change-research/Climate-Atlas-Development)
  is the private application-development and deterministic-build repository.
- this repository is only the checksum-locked public projection.

See [PUBLICATION.json](PUBLICATION.json),
[SITE-FILE-MANIFEST.json](SITE-FILE-MANIFEST.json), and
[SHA256SUMS.txt](SHA256SUMS.txt) for the exact publication identity and bytes.

## Rehosting and recovery

The browser needs no paid API, secret key, or live scientific-data service.
After verifying `SHA256SUMS.txt`, serve the contents of `site/` from any static
host with `site/index.html` as the entry point. Detailed migration instructions
are in [MIGRATION.md](MIGRATION.md).

## Copyright and licensing

Copyright © 2026 John Luikart. All rights reserved.

No license is granted for project-authored code, text, design, branding,
compiled assets, or data compilations except where expressly stated. Public
visibility and GitHub's interface do not make the project open source or open
content. Third-party scientific data and software retain their own licenses
and attribution requirements; see
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

