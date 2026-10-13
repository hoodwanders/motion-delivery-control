# Studio source pointer

**Status:** Built 13 October 2026.  
**Role:** Delivery-standards source for questions v2, by reference (not copied).

## Location

`C:\Users\A-Med\Desktop\animation-studio`

## Why by reference

- The studio folder is large (includes `.git/`, `node_modules/`, film renders) and live. Copying it into `sources/` would duplicate bytes, risk drift, and break the minimal-folder rule.
- Per `_skills/cross-project-references.md`: name the exact artefact and path; do not duplicate contents.
- The locked index `../../01-source-and-question-lock/output/delivery-standards-source-index.md` (DS-1–DS-8, approved 13 October 2026) is the authority for what counts as source. This pointer resolves those DS IDs to files.

## DS resolution

| Source ID | File | Lines / section |
|---|---|---|
| DS-1 | `workflows/studio/CONTEXT.md` | :4 — code-drawn films, captured to MP4 |
| DS-2 | `workflows/studio/03-design/CONTEXT.md` | :21-24 — Stop 1 show + `approve --stage plan` |
| DS-3 | `workflows/studio/04-shot-plan/CONTEXT.md` | :18-22 — board agreement + Stop 1 staleness |
| DS-4 | `workflows/studio/06-build/CONTEXT.md` | :15-22 — code outputs; check is not master; MP4 location rule |
| DS-5 | `workflows/studio/07-capture/CONTEXT.md` | :12-29 — preview vs render, watch+listen, delivery package, completion, Stop 2, never publishes, QA != acceptance |
| DS-6 | `workflows/studio/cli/tools/CONTEXT.md` | :22-40 — hash-bound approvals, repair withdraws, production.json, QA statuses, do not publish |
| DS-7 | `workflows/studio/projects/CONTEXT.md` | :10-14 — pointers only; approvals in production.json |
| DS-8 | `package.json` | :13-24 — CLI verbs |

## Rule

If the studio folder moves, update this pointer and re-verify DS line numbers. Do not invent specs absent from these files.
