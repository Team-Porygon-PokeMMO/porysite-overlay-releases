# Team Porygon Overlay — releases

Compiled builds of the **Elite Four desktop overlay** for PokeMMO, plus the
manifest the app reads to update itself.

**There is no source code here.** This repository exists only because the
project's source repository is private, and a private repository's release
assets return `404` to anyone without access — so neither a player's download
nor the app's own update check could ever reach them. The binaries published
here were already being served from a public website; only their home moved.

## What is in a release

| File | Who reads it |
|---|---|
| `*-setup.exe` | Players, downloading for the first time |
| `latest.json` | The app's updater, and the download page on the site |
| `*.sig`, `*.nsis.zip` | The updater — not meant to be downloaded by hand |

Every update is signed. A payload that does not verify is refused rather than
installed, whatever it claims to be.

## Getting it

Download from **the site's own page**, not from here:
<https://team-porygon-pokemmo.pages.dev/elitefour-overlay> — it explains the
Windows SmartScreen warning you will see, since the app is not code-signed.

Installing by hand is a one-time thing. After that the app updates itself.

## Issues

Report problems on the site or to Team Porygon. This repository takes no
issues or pull requests; it holds build output only.

---

Not affiliated with or endorsed by PokeMMO.
