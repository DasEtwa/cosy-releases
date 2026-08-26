# Cosy Releases 🌱

Public distribution repository for **Cosy** iOS builds.

The game source code lives in a separate private repository. This repository intentionally contains only public distribution metadata, the SideStore source, the GitHub Pages site and released IPA binaries.

## SideStore

GitHub Pages publishes the SideStore source at:

`https://dasetwa.github.io/cosy-releases/source.json`

The source may exist before the first public Cosy build; until then its app list is intentionally empty.

## Releases

Cosy IPA files should be published as **GitHub Release assets**, not committed directly to the Git history.

Suggested naming:

```text
Cosy-v0.0.1.ipa
Cosy-v0.0.2.ipa
```

When a build is published, add/update the corresponding entry in `site/source.json` so SideStore can discover the release.

## Repository boundary

This repository is **not** the Cosy source repository.

Do not publish here:

- Rust game/runtime source
- renderer internals
- private game assets
- signing certificates, provisioning profiles or secrets
- private build artifacts that are not intended for distribution

## Rights

Cosy and its distributed binaries/assets are proprietary unless explicitly stated otherwise. See [`LICENSE`](./LICENSE).
