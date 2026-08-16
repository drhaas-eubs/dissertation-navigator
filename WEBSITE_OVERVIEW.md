# EUBS Dissertation Navigator — Complete Website Overview

*A structured GitHub Pages site for the MBA Dissertation and BBA Dissertation at EU Business School, Munich. Supervision: Dr. Hildegard HAAS.*

House style: navy `#16263F`, gold `#E0A126`, Arial. No build step — pure HTML/CSS/JS + PDFs.

---

## 1. Top navigation (identical on all 7 pages)

```
Home  ·  I · Proposal  ·  II · BBA Dissertation  ·  MBA Dissertation  ·  III · Defence  ·  Frameworks  ·  Authors
```

The active tab is highlighted in gold on each page. Bachelor is listed before MBA; both sit under Part II with the numeral shown once.

---

## 2. The seven pages

### `index.html` — Home / cover
- **Hero:** "The Dissertation Navigator", naming the MBA Dissertation and BBA Dissertation.
- **Choose your track** — two side-by-side panels:
  - **MBA Dissertation** (navy): 16,000 words · 80–100 references · 83% pass · 60/20/20 weighting → opens the dissertation page.
  - **BBA Dissertation** (gold): 14,000 words · 50–80 references · 70% pass · 70/30 weighting → opens the BBA page.
  - Navy callout: the hard gates apply to both.
- **Work through it in order** — three cards: Part I Proposal, Part II Dissertation, Part III Defence.
- **Galleries & the Research Methods Slibrary** — cards for Frameworks, Authors, BBA.

### `part1-proposal.html` — Part I · The Proposal
- **Registration information** — table incl. the promoter field (Dr. Hildegard HAAS).
- **The proposal — seven parts** — the seven proposal sections, each as a figure card (three-tier: card → modal → A4 sheet):
  1. Proposed Dissertation Title
  2. Research Question or Hypothesis (~100 words)
  3. Review of Literature / Background (~500 words)
  4. Research Methodology
  5. Selected Bibliography (max 20)
  6. Research & Writing Timeline
  7. Ethics
- **The signature block** — Promoter / Coordinator / Department table.

### `part2-dissertation.html` — Part II · The Dissertation
- **The MBA targets** — stat tiles: 16,000 words · 80–100 references · 83% pass · 60/20/20. Bachelor line: 14,000 / 50–80 / 70% / 70-30. Per-chapter word budget.
- **The compliant six-chapter structure** — an **8-entry numbered accordion**:
  1. **Introduction** (~1,800 words)
  2. **Background & Literature Review** (~4,800 words)
  3. **Methodology** (~2,800 words)
  4. **Findings / Results** (~4,000 words)
  5. **Discussion** (~1,600 words, standalone)
  6. **Conclusion** (~1,000 words)
  7. **References** — Harvard list of all frameworks & methods sources
  8. **Appendix** — 8.1 List of Figures · 8.2 List of Tables · 8.3 Other materials (questionnaire, consent, transcripts, AI Annex)
  - Each of chapters 1–6 opens to reveal: a lead, "What this chapter must contain" (sub-sections), a **nested "Frameworks & Slibrary sheets" accordion** (opens the relevant A4 methods sheets), and an AMBER self-check.
- **The paradigm chain (Chapter 3)** — ontology→methods coherence table.
- **How it is marked** — rubric weighting table (60/20/20).
- **Three things that are not optional** — Ethics Agreement, AI Annex, Harvard (traffic-light panel).

### `part3-defense.html` — Part III · The Jury Defence
- **It's a defence, not a presentation** — mindset + ownership callout.
- **Build it as thumbnails first (J.D. Meier)** — the 9 defence slides, each as a figure card (card → modal → A4 sheet):
  1. Title Slide · 2. Research Objective · 3. Significance · 4. Research Question(s) · 5. Literature Review · 6. Methodology · 7. Findings/Results · 8. Discussion & Conclusion · 9. Reflection on the Process
- **One message per slide (Kurt Bostelaar)** — do/avoid two-column.
- **What the oral defence is scored on** — criteria table.

### `bba.html` — BBA Dissertation
- **The BBA targets** — 14,000 words · 50–80 references · 70% pass · 70/30.
- **What changes, what doesn't** — full MBA-vs-BBA comparison table.
- **Use the main pages** — cards linking to Parts I–III and Frameworks.

### `frameworks.html` — Framework Gallery
- **Research Methods Slibrary** — 16 sheets (with thumbnail figures) in four groups: A Foundations · B Design & Sampling · C Data Collection & Analysis · D Writing & Integrity.
- **26 framework cards** across 7 categories, each with figure + three-tier drill-down:
  - Strategy & Competitive (6): Five Forces, Value Chain, RBV/VRIN, Dynamic Capabilities, Disruptive Innovation, Business Model Canvas
  - Technology Adoption (4): TOE, TAM, UTAUT, Diffusion of Innovations
  - Change & Transformation (3): Kotter 8-Step, Digital Transformation Playbook, IT-Enabled Transformation
  - Innovation & Entrepreneurship (3): Design Thinking, Effectuation, TAM·SAM·SOM
  - Environmental Scan (3): PESTEL, SWOT, Balanced Scorecard
  - Research Design (4): Research Onion, Case Study, Building Theory from Cases, Mixed Methods
  - Data Analysis (3): Thematic Analysis, Grounded Theory, Qualitative Data Analysis
- Filter box + category pills. Every card: figure → quick-look modal (red definition, bullets, Harvard reference) → full A4 PDF.

### `authors.html` — Authors Gallery
- The seminal authors behind the frameworks, grouped, each with the originating Harvard reference — so students cite the originator, not a second-hand summary.

---

## 3. The three-tier "Slibrary" drill-down (used throughout)

Every reference item works the same way:
1. **Thumbnail card** — on-brand SVG figure + name + short definition + badge.
2. **Quick-look modal** — figure, **red definition**, key bullets, Harvard reference, "View Full A4 Reference Sheet" button. Closes on ×, backdrop, or Esc.
3. **Full A4 PDF** — navy/gold sheet with red definition, gold-bulleted key points, Harvard reference, "Dr. Hildegard HAAS" footer.

---

## 4. A4 reference sheets (57 PDFs total)

- **16 Slibrary methods sheets** (`slibrary/`): 01 Primary & Secondary · 02 Paradigms · 03 Philosophy · 04 Reasoning · 05 Designs · 06 Qual/Quant/Mixed · 07 Sampling · 08 Validity · 09 Data Collection · 10 Thematic · 11 Statistics · 12 Coding · 13 Harvard · 14 Literature Review · 15 Ethics · 16 Integrity & AI.
- **19 framework sheets** (`frameworks/`): the strategy/tech/change/scan frameworks that don't reuse a methods sheet.
- **22 chapter/proposal/defence sheets** (`sheets/`): ch1–ch6 · p1–p7 · d1–d9.

---

## 5. Hard gates & key rules baked in across the site

- **Ethics Agreement** — signed before any data collection (RED gate).
- **AI Annex** — PowerPoint, one screenshot per source, working OneDrive link.
- **Harvard referencing** — throughout, in-text and list matched both ways.
- **Standalone Discussion chapter** — separate from Findings.
- **Word counts** — MBA 16,000 · BBA 14,000 (introduction to conclusion; front matter, references, annexes excluded).
- **References** — MBA 80–100 · BBA 50–80.
- **Pass marks** — MBA 83% · BBA 70%.

---

## 6. Integrity check (automated, current)

| Check | Result |
|---|---|
| Broken internal links | ✓ none (all resolve) |
| Promoter name | ✓ "Dr. Hildegard HAAS" everywhere · 0 wrong forms |
| Word counts | ✓ MBA 16,000 · BBA 14,000 · 0 stale figures |
| Navigation | ✓ identical order on all 7 pages |
| Slibrary cards / modals | 16 / 16 |
| Framework cards / modals | 26 / 26 |
| Chapter accordions | 8 (6 chapters + References + Appendix) |
| Nested framework accordions | 6 (chapters 1–6) |
| Proposal cards | 7 · Defence cards | 9 |
| Total files | 75 (7 HTML · 1 CSS · 57 PDF · build scripts) |

---

## 7. To publish (GitHub Pages)

Upload the whole `dissertation-navigator` folder — **keeping the `slibrary/`, `frameworks/` and `sheets/` sub-folders alongside the HTML** — to a repo, then Settings → Pages → `main` branch → `/ (root)`. Live within a minute or two. A cross-link to the MARTI301 site is in every page footer.

---

## 8. Two open items for your confirmation

1. **Chapter → Slibrary mapping** (part2 nested accordions): I mapped which methods sheets appear under each chapter by standard placement — glance at chapters 5 and 6 especially and tell me if any sheet should move.
2. **Kurt Bostelaar message strategy** (Part III) is written as a house synthesis of documented communication principles, not a verbatim published model — swap in his handout if you have one.


---

## UPDATE — consistent accordion across all four content pages

Part I (Proposal), Part II (MBA Dissertation), BBA Dissertation and Part III (Defence)
now share the **same numbered-accordion structure**, each entry expandable with a nested
"Frameworks & Slibrary sheets" accordion inside:

| Page | Accordion entries | Nested Slibrary accordions |
|---|---|---|
| Part I · Proposal | 7 (the proposal sections) | 6 |
| Part II · MBA Dissertation | 8 (6 chapters + References + Appendix) | 6 |
| BBA Dissertation | 8 (6 chapters + References + Appendix, BBA word targets) | 6 |
| Part III · Defence | 9 (the defence slides) | 7 |

Each entry: title + meta in the summary (numbered circle, gold +/- toggle) → expands to a
lead, "What this section/chapter must contain", the nested Slibrary accordion, and a
"View Full A4 Reference Sheet" button. The old flat card galleries and step lists are removed.


---

## UPDATE — consistency polish

- **Part II** renamed to **MBA Dissertation** throughout (title, eyebrow, H1, nav) — was "The Six-Chapter Dissertation".
- **BBA** renamed from "BBA Variant" to **BBA Dissertation** (title, eyebrow) — matches the nav.
- Index cards updated: "The Dissertation" → "MBA Dissertation", "BBA Variant" → "BBA Dissertation".
- Framework Gallery intro made inclusive of both tracks ("your MBA or BBA dissertation").
- BBA page: removed the now-redundant link back to the MBA six-chapter structure (BBA has its own full chapter accordion); kept Proposal, Defence and Frameworks shared links.
- All stale terms ("Variant", "BBA page", "Six-Chapter") removed. All links resolve, all tags balanced, promoter name correct.
