# Upstream provenance

- Original project: https://github.com/jellyfin/jellyfin-androidtv
- Upstream base: `08ccb98093272babb26d10dd6f0dde358d8324c9`
- License: GNU General Public License v2; see `LICENSE` and source notices.
- Original contributors: see `CONTRIBUTORS.md` and the upstream project's history.

This repository is a source snapshot with a fresh history. Upstream copyright,
license notices, contributor attribution and original assets are preserved.

The functional difference from this upstream revision is the removal of the
`KnownDefects.hevcDoviHdr10PlusBug` block in
`app/src/main/java/org/jellyfin/androidtv/util/profile/deviceProfile.kt`.
The removed block excluded `DOVI_WITH_HDR10_PLUS` and
`DOVI_WITH_ELHDR10_PLUS` from the advertised video range types.

Other snapshot changes are project documentation, expanded ignore rules
for local credentials and build artifacts, and build/test/lint/wrapper-check
workflow triggers extended to include `main`. Upstream release publishing and
maintenance jobs retain their Jellyfin-owner guards.
