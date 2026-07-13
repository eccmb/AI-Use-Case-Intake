# Changelog

## v0.4 — 2026-07-12 (current)

- Split into two editions for confidentiality: public **submitter edition** (`index.html`) contains intake, triage, routing, answer review, and export only — no weighting, scoring, or portfolio logic exists in the file; internal **reviewer edition** (kept out of the repository) retains full scoring, weight scenarios, portfolio ranking, rescore workflow, and imports submitter JSON exports directly
- Submitter review step now shows a full answer summary instead of a score preview
- New "My Submissions" tab: personal record of all submissions with follow-up counts, read-only detail view, JSON/CSV export of every answer
- `.gitignore` excludes internal reviewer materials and working drafts from the repository

## v0.3 — 2026-07-12

- Full 0–5 scale on all 19 questions; every value has a plain-language explanation (2s and 4s newly drafted; original framework defined 1/3/5 only)
- 0 = "Not sure / NA" available on every question; counts as 0 and flags the item for follow-up interview and rescore
- All questions rewritten from the submitter persona's perspective — no technical jargon (API, MCP/A2A, PII, HITL moved to docs/Build_Reference.md)
- Productivity question updated to measure total time saved across all affected staff, not a single person
- New tabs: Instruction (end-user guide) and Scoring Explanation (plain-language scoring guide)
- Per-submission Detail view: every original answer visible, evaluator rescore with side-by-side audit trail
- CSV/JSON exports retabulation-ready: submitted + rescored value per question, triage answers, follow-up counts
- Repository packaged for GitHub: index.html, README, docs/, archive/

## v0.2 — 2026-07-12

- Two-layer question design (plain intake / technical evaluator) — superseded by v0.3 single 0–5 scale
- Evaluator override scores (effScores) and uncertainty flags introduced

## v0.1 — 2026-07-12

- Initial prototype: triage wizard with fast-track vs. full-evaluation routing, 4-category weighted evaluation, quant synergy multiplier (Option 2), four weighting scenarios (Efficiency default), portfolio ranked table + value-vs-feasibility 2×2, localStorage persistence, CSV/JSON export/import
- Scoring math verified against framework worked examples (Use Case A: 1.0x/7; Use Case B: 1.4x/14)
