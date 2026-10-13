# Source Note

## Delivery-standards source

- Authority: `delivery-standards-source-index.md` (DS-1–DS-8, approved 13 October 2026).
- Location at run time (paired-20261013-v2-01): `C:\Users\A-Med\Desktop\animation-studio` (HG-owned studio folder).
- Vendored 14 October 2026: `motion-delivery-folder/sources/vendor-studio/` — verbatim copies of the 8 locked DS files (all hashes match originals). Contest review uses these copies; the absolute path is no longer required.
- Resolution: `motion-delivery-folder/sources/studio-source-pointer.md` maps each DS ID to vendored file + lines (e.g. `sources/vendor-studio/workflows/studio/CONTEXT.md:4`).
- Mode: vendored minimal copy — only the 8 DS files; no `.git/`, `node_modules/`, or renders.

## Why only 8 files are vendored

- The full studio folder is HG-owned working material and too large to vendor.
- Absolute paths (e.g. `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\...`) are preserved verbatim in the 13-Oct raw treatment record as evidence of what was cited then. They are not rewritten — the raw record is unedited. New runs cite `motion-delivery-folder/sources/vendor-studio/...`.

## What judges can verify directly in this repo (no studio folder needed)

- Question-to-source routes: `questions-v2.md` source-route column + `motion-delivery-folder/coverage-map.md` (15/15 mapped, Q15 explicit unavailability).
- Citation shape: every treatment Q1–Q14 answer cites file + line/section; Q15 cites the coverage route and states the exact unavailability sentence.
- Source index contents: `delivery-standards-source-index.md` records the rule text relied on per DS ID.
- Control behaviour: control raw states studio specifics unavailable and avoids inventing studio paths, commands or specs.

## To reproduce fully

- Use the vendored copies under `motion-delivery-folder/sources/vendor-studio/`, then re-run the v2 questions under the same model / order / settings. No studio-folder access needed.

## Line drift

- Line numbers verified 13 October 2026 (pointer) and 14 October 2026 (vendored copies, hash-matched). If the live studio folder moved since, the vendored copies remain the locked evidence.

## Results note

- `paired-20261013-v2-01` treatment ran against the pointer version. The folder content is materially identical (byte-identical DS text), but citation paths changed to `sources/vendor-studio/...`. A fresh paired run with the vendored folder is required before the 28/30 treatment total can be claimed for this folder version.
