# Studio source pointer

**Status:** Fixed 14 October 2026 — vendored copies in-folder; checkable on GitHub.
**Role:** Delivery-standards source for questions v2, vendored in `vendor-studio/` (verbatim copies).

## Location

- Vendored (authoritative for contest): `sources/vendor-studio/` in this folder.
- Original: `C:\Users\A-Med\Desktop\animation-studio` (HG-owned; not required for review).

## Why vendored

- Contest owners check GitHub; an absolute `C:\...` path is not portable or reviewable.
- Stage 2 instruction 1 requires source material in `output/motion-delivery-folder/sources/`.
- Only the 8 locked DS files are vendored (minimal-folder rule kept); no `.git/`, `node_modules/`, or renders copied.
- Copies verified byte-identical 14 October 2026 (all 8 hashes match originals).
- Per `_skills/cross-project-references.md`: name the exact artefact and path; vendored paths below preserve original relative paths under `vendor-studio/`.

## DS resolution (vendored paths; line numbers verified 13–14 October 2026)

| Source ID | File | Lines / section |
|---|---|---|
| DS-1 | `vendor-studio/workflows/studio/CONTEXT.md` | :4 — code-drawn films, captured to MP4 |
| DS-2 | `vendor-studio/workflows/studio/03-design/CONTEXT.md` | :21-24 — Stop 1 show + `approve --stage plan` |
| DS-3 | `vendor-studio/workflows/studio/04-shot-plan/CONTEXT.md` | :18-22 — board agreement + Stop 1 staleness |
| DS-4 | `vendor-studio/workflows/studio/06-build/CONTEXT.md` | :15-22 — code outputs; check is not master; MP4 location rule |
| DS-5 | `vendor-studio/workflows/studio/07-capture/CONTEXT.md` | :12-29 — preview vs render, watch+listen, delivery package, completion, Stop 2, never publishes, QA != acceptance |
| DS-6 | `vendor-studio/workflows/studio/cli/tools/CONTEXT.md` | :22-40 — hash-bound approvals, repair withdraws, production.json, QA statuses, do not publish |
| DS-7 | `vendor-studio/workflows/studio/projects/CONTEXT.md` | :10-14 — pointers only; approvals in production.json |
| DS-8 | `vendor-studio/package.json` | :13-24 — CLI verbs |

## Rule

Original relative paths (`workflows/studio/...`, `package.json`) are preserved under `vendor-studio/`. Cite as `sources/vendor-studio/<original path>:<lines>` (e.g. `sources/vendor-studio/workflows/studio/CONTEXT.md:4`). If the studio folder moves, re-vendor and re-verify hashes. Do not invent specs absent from these files.
