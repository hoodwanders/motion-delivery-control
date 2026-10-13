# Delivery Standards Source Index

**Status:** Approved — locked.  
**Source:** `C:\Users\A-Med\Desktop\animation-studio` (HG-owned studio folder, no client spec).
**Approved by HG:** Yes — chat, 13 October 2026.

| Source ID | Title | Location | Covers | Notes |
|---|---|---|---|---|
| DS-1 | Studio purpose | `workflows/studio/CONTEXT.md:4` | Code-drawn films, captured to MP4 | Delivery format basis; no broadcast spec |
| DS-2 | Stop 1 — plan approval | `workflows/studio/03-design/CONTEXT.md:21-24` | Show premise/key moments/look/board/exceptions; end turn; `approve --stage plan --note "<their words>"` | Owner-words approval only |
| DS-3 | Shot-plan agreement + staleness | `workflows/studio/04-shot-plan/CONTEXT.md:18-22` | `shots.md` + `storyboard.md` must exist, no TODO, agree; edit to brief/references/design makes Stop 1 stale | Approval trigger basis |
| DS-4 | Build outputs; check vs master | `workflows/studio/06-build/CONTEXT.md:15-22` | Code in `<id>/`, `project.json`; check/stills/strip are not master; renders go to `07-capture/<id>/output/`; do not write MP4s in build | Location + master distinction |
| DS-5 | Capture delivery package | `workflows/studio/07-capture/CONTEXT.md:12-29` | `preview` (no approval) vs `render` (needs current plan approval); watch continuously + listen or document silence; `<id>/output/` + `review.md` + `playback-review.json` + `build-log.md` with each video SHA-256; completion = current master, no QA failures, complete playback, `review.md` no TODO naming SHA-256; file presence is not acceptance; Stop 2 release approval; never publishes; QA is not acceptance | Core handoff + QC + approval basis |
| DS-6 | CLI gates and state | `workflows/studio/cli/tools/CONTEXT.md:22-40` | Approvals bound to hashes; `repair` withdraws both; state in `projects/<id>/production.json`; QA PASS/FAIL/WARN/NOT APPLICABLE/NOT TESTED is not creative acceptance; missing evidence never passes; do not publish/upload | Version/hash + gate basis |
| DS-7 | Film log | `workflows/studio/projects/CONTEXT.md:10-14` | Pointers only; `production.json` written by CLI; approvals live there | Approval record location |
| DS-8 | CLI verbs | `package.json:13-24` | `status/preview/render/qa/approve/repair/check/stills/strip/audio` | Command vocabulary only; not a standard |

## Rule

Add a row only for source material actually supplied by HG. Rows above are extracted verbatim from HG's studio folder on 13 October 2026; nothing invented. Approved by HG chat 13 October 2026 — Stage 1 source lock complete.
