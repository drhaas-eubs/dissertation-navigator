# Dissertation Navigator — EU Business School

A static GitHub Pages site giving Bachelor (BBA) and MBA students a structured,
three-part workspace for the dissertation journey, built on the official EUBS
requirements. House style: navy #16263F, gold #E0A126, Arial.

## Pages
- `index.html` — landing page (three parts + galleries + BBA)
- `part1-proposal.html` — Part I · The Proposal (EUBS registration form, 7 sections, sign-off)
- `part2-dissertation.html` — Part II · The Dissertation (six-chapter structure, paradigm chain, rubric, hard gates)
- `part3-defense.html` — Part III · The Jury Defence (J.D. Meier thumbnail storyboard + Kurt Bostelaar message strategy)
- `frameworks.html` — Framework Gallery + the 16-sheet Research Methods Slibrary
- `authors.html` — Authors Gallery (seminal references, grouped)
- `bba.html` — BBA variant (Bachelor targets + MBA-vs-BBA table)
- `style.css` — shared house style
- `slibrary/` — 16 A4 reference-sheet PDFs, opened from the cards on `frameworks.html`.
  Keep this folder alongside the HTML so links resolve. Sheets:
  01 Primary & Secondary · 02 Paradigms · 03 Philosophy · 04 Reasoning ·
  05 Designs · 06 Qual/Quant/Mixed · 07 Sampling · 08 Validity ·
  09 Data Collection · 10 Thematic · 11 Statistics · 12 Coding ·
  13 Harvard · 14 Literature Review · 15 Ethics · 16 Integrity & AI.

## Deploy to GitHub Pages

**Option A — new repo**
1. Create a repository named `dissertation-navigator` (analogous to your `business-plan-navigator`).
2. Upload every file in this folder (including the `slibrary/` folder) to the repo root.
3. Settings → Pages → Source: `main` branch, `/ (root)` → Save.
4. Live at `https://drhaas-eubs.github.io/dissertation-navigator/` within a minute or two.

**Option B — add to your existing `marti301` repo**
1. Copy this folder into the repo (e.g. as `/dissertation/`).
2. Served at `https://drhaas-eubs.github.io/marti301/dissertation/`.
3. A cross-link to the MARTI301 site is already in the footer of every page;
   add a reciprocal link from your MARTI301 landing page.

No build step, no dependencies — pure HTML/CSS/JS + PDFs.

## Notes for the supervisor
- Promoter is written throughout as **Dr. Hildegard HAAS** (surname in capitals),
  in every page and in every slibrary PDF footer.
- All framework and slibrary references follow Harvard style but should be
  **verified before students cite them** — a standing "Verify every source yourself"
  line is on every PDF and a warning is on `frameworks.html` and `authors.html`.
- Kurt Bostelaar's "message strategy" (Part III) is presented as a house synthesis of
  documented communication principles, not a verbatim published model — swap in his
  actual handout if you have one (a note to that effect is on the page).
- MBA figures: ~16,000 words, 80–100 references, 83% pass, 60/20/20 weighting.
  BBA figures: 12,000–14,000 words, 50–80 references, 70% pass, 70/30 weighting.
  Both share the six-chapter structure, standalone Discussion chapter, and the two
  hard gates (signed Ethics Agreement; AI Annex with working OneDrive link).

## Regenerating the slibrary PDFs
The 16 PDFs are built from `slib_engine.py` + `specs.py` (ReportLab). To change a sheet,
edit its entry in `specs.py` and re-run `python3 slib_engine.py`.


## Framework Gallery — three-tier Slibrary pattern
Every framework card on `frameworks.html` now works as a three-tier drill-down,
matching the Research Methods Slibrary:
1. **Thumbnail card** — on-brand SVG figure + name + author + red definition + FRAMEWORK badge.
2. **Quick-look modal** — the figure, the red definition, key bullets, a Harvard reference,
   and a "View Full A4 Reference Sheet" button. Opens on click; closes on ×, backdrop click, or Esc.
3. **Full A4 PDF** — in `frameworks/` (19 sheets). Frameworks that duplicate a methods sheet
   (Research Onion, Case Study, Building Theory from Cases, Mixed Methods, Thematic Analysis,
   Grounded Theory, QDA) point instead to the matching Slibrary sheet in `slibrary/`.

The 26 framework cards, their SVG figures and A4 PDFs are generated from `fw_data.py`,
`fw_figures.py` and `fw_build.py`. To add or edit one, edit its entry in `fw_data.py`
(and its figure in `fw_figures.py`), then re-run `python3 fw_build.py`.


## Thumbnail figures across the whole companion
Every reference item now has an on-brand SVG thumbnail and the three-tier drill-down
(figure card → quick-look modal with red definition + bullets + Harvard reference → full A4 PDF):

- **16 Research Methods Slibrary** sheets — figures added to cards and modals (`frameworks.html`).
- **26 Framework Gallery** cards — figures + own A4 sheets in `frameworks/`.
- **6 dissertation chapters** — figure cards on `part2-dissertation.html` above the detailed
  accordions; A4 sheets in `sheets/` (ch1–ch6).
- **7 proposal sections** — figure cards on `part1-proposal.html`; A4 sheets in `sheets/` (p1–p7).
- **9 jury-defence stages** — figure storyboard cards on `part3-defense.html`; A4 sheets in
  `sheets/` (d1–d9).

Total A4 reference sheets: 16 (slibrary) + 19 (frameworks) + 22 (chapters/proposal/defence) = 57.

Figures are generated from `slib_figures.py`, `fw_figures.py` and `cpd_figures.py`; content and
PDFs from `*_data.py` + `*_build.py`. Edit the data/figure module and re-run the matching build
script to regenerate.
