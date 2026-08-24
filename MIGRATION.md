# Static-site migration and restoration

This repository is deliberately host-portable. The deployed site has relative
URLs, local runtime data, no browser credentials, and no dependency on a live
scientific publisher.

## Verify

From the repository root:

```sh
sha256sum -c SHA256SUMS.txt
jq -r '.files[] | "\(.sha256)  site/\(.path)"' \
  SITE-FILE-MANIFEST.json | sha256sum -c -
```

Confirm that `PUBLICATION.json` identifies 40-character Research and
Development commits and says both runtime credential and publisher
dependencies are false.

## Serve on another static host

Publish the contents of `site/` as the host's document root. Do not publish the
private Research or Development repositories. A local smoke test is:

```sh
python3 -m http.server 4173 --bind 127.0.0.1 --directory site
```

Then open `http://127.0.0.1:4173/`. All scientific images, GeoJSON, metadata,
notices, and licenses are already inside `site/`.

## Recreate under another GitHub account

1. Restore the public Git bundle or mirror from the latest verified Google
   Drive checkpoint.
2. Push all refs into a new repository.
3. Confirm the exact main commit and rerun the public artifact workflow.
4. Configure GitHub Pages to use GitHub Actions, or publish `site/` through a
   different static host.
5. Preserve the original publication receipt and create a new dated migration
   receipt for any changed repository or deployment URL.

Git exports do not contain GitHub Pages settings, Actions artifacts/logs,
issues, pull-request discussions, Releases, or secrets. The Drive checkpoint
therefore stores GitHub metadata and restoration notes separately. Credential
values are never backed up; only required secret names and re-entry steps may
be recorded.

