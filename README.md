# GS Media – XCMate EPG

Public delivery endpoint for approved XMLTV programme-guide exports from GS Media EPG Hub. This repository contains no IPTV access credentials, streaming playlists or video streams.

## Client interface

- Manifest: `https://raw.githubusercontent.com/artattakk-creator/xcmate-epg-public/main/manifest.json`
- Schema version: 5 (`gsmedia-hub-github-v3`).
- Consume only manifests with status `PUBLIC_READY`. Use the `download_url` and SHA-256 of the selected profile and variant in `files`; validate size, digest, GZIP and XMLTV before replacing local LastGood data.
- The public reader does not require a GitHub token. Provider EPG remains independent.
- Intended profiles: all, de, at, en, es, pl, each in standard and artwork variants as enabled in the hub.
- Verified exports are distributed as GitHub Release assets; the hub maintains the current manifest and rotates its own superseded releases.

## Publication status

Initial setup only. No EPG datasets have been released. Publication requires a verified fresh import, a clean export and confirmed rights for all included data, logos, metadata and image references. Third-party content is not licensed by this README.
