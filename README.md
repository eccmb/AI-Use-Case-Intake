# AI Use Case Intake

One front door for AI ideas across every business function. Submitters describe an idea in plain language; the system routes it — self-service builds fast-track through, everything else completes a short questionnaire for the AI portfolio team to review and prioritize.

**No install. No dependencies. Open `index.html` in any browser.**

## What it does

- **Triage & routing** — four quick questions classify who benefits and who builds. Individual/team ideas buildable with approved tools are registered for visibility and skip the questionnaire. Anything needing IT, external agencies, or touching customer data / regulated data / public content completes the full questionnaire.
- **Plain-language questionnaire** — 19 questions across four topics: strategic alignment, business impact and value, feasibility and readiness, risk and safeguards. Every answer 0–5 is explained in plain terms; 0 = "Not sure" is always valid and flags the item for a follow-up conversation.
- **Follow-up workflow** — "Not sure" answers are revisited with the submitter so assessment reflects accurate information, not gaps. Original answers stay on record.
- **Complete answer capture** — exports include the submitter's answer to every question plus all triage choices, so nothing is ever re-entered.

## How submissions are evaluated

Evaluation, scoring, and prioritization are performed by the AI portfolio review team in a separate internal tool, against current company priorities. This public intake app contains no scoring or prioritization logic.

## Data model (prototype)

Data lives in the browser's local storage — nothing leaves the machine. Each visitor gets their own local data. Submitters use **Export JSON** on the My Submissions tab and send the file to the portfolio owner. Server-backed storage is the planned next step; the JSON export is the migration path.

## Hosting on GitHub Pages

Settings → Pages → Deploy from branch → `main`, root folder. The site serves from `index.html` automatically. Note: public Pages sites are visible to anyone — confirm with IT before enabling.

## Repository structure

```
index.html      The intake application (single file, submitter-facing)
CHANGELOG.md    Version history
```

Internal materials (reviewer tooling and methodology reference) are maintained separately and excluded from this repository via `.gitignore`.

---

The framework guides the reviewers; the questionnaire is the front door. Plain questions in, complete answers out.
