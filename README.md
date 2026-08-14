# Kometa Overlay Assets

PNG images, fonts, and sprites used by the [kometa-overlay-configs](https://github.com/Naveen11695/kometa-overlay-configs) overlay YAML files.

## Contents

- **Root badges** — 4K, HDR, Dolby Vision, NEW, RETURNING, ENDED, network logos
- **r0–r100.png** — Color-coded rating score sprites
- **images/media_info/** — Codec, resolution, and edition badges (DIGITAL+, DTS, Atmos, etc.)
- **images/gradients/** — Backdrop gradients for media-info overlays
- **images/audience_score/** — Rating chip backgrounds
- **network-top-left/** — Network logos (top-left placement)
- **fonts/** — Custom fonts for overlay text (e.g. Colus-Regular for animetafill)

## Setup

Place the contents of this repo inside your Kometa `config/overlays/` directory so overlay YAML `file` paths (e.g. `config/overlays/4K-HDR.png`) resolve correctly. The overlay YAML definitions live in the companion [kometa-overlay-configs](https://github.com/Naveen11695/kometa-overlay-configs) repo — see its README for full setup instructions.

```bash
# After cloning both repos
cp -r /tmp/kometa-overlay-assets/. /volume1/docker/kometa/config/overlays/
```

## Screenshots

Example overlays applied in Plex are shown in the [kometa-overlay-configs README](https://github.com/Naveen11695/kometa-overlay-configs#screenshots).

## Sources & Upstream Repos

Many assets in this repo are derived from or complement upstream community projects:

| Project | Repo URL | What it provides |
|---------|----------|------------------|
| **jmxd overlays** | [jmxd/Kometa](https://github.com/jmxd/Kometa) | Media-info badge images (`images/media_info/`, gradients, audience score chips) |
| **TSSK-Kabeb** | [netplexflix/Overlays](https://github.com/netplexflix/Overlays/tree/main/TSSK-Kabeb) | Network logos and trending badges (some configs load these via remote URL instead of local copies) |
| **kometa-overlay-configs** | [Naveen11695/kometa-overlay-configs](https://github.com/Naveen11695/kometa-overlay-configs) | YAML files that reference these assets |
| **Kometa** | [Kometa-Team/Kometa](https://github.com/Kometa-Team/Kometa) | Application that applies overlays to Plex posters |

See the [kometa-overlay-configs Sources table](https://github.com/Naveen11695/kometa-overlay-configs#sources--upstream-repos) for the full list of upstream projects (UMTK, animetafill, MDBList, etc.).

## Excluded

Personal poster backups and Synology system files are not included in this repo.
