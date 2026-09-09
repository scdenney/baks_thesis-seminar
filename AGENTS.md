# BAKS Thesis Seminar - Project Context

> Durable rules and orientation only. Session state lives in `HANDOFF.md` (newest entry on top, append-only). Prose conventions follow the `sci-edit` skill (writing-toolkit); only local exceptions are listed here.

---

## Project Overview

**Repository:** baks_thesis-seminar
**Purpose:** GitHub Pages website for the BA-Eindwerkstuk Seminar (5723VKO1Y)
**Program:** BA Korean Studies, Leiden University
**Term:** AY2025-2026 (Spring)
**Instructor:** Dr. Steven Denney (s.c.denney@hum.leidenuniv.nl)

---

## Design decisions

- Copied design from BA2 Digital Korea site (https://github.com/scdenney/ba2_digital-korea)
- Navigation: Home | Syllabus | Presentations | Assignments | Style Guide | Protocol
- Leiden University branding with blue header and gold accent
- Syllabus page uses sidebar TOC for easy navigation

---

## Site Structure

```
baks_thesis-seminar/
├── _config.yml                 # Jekyll configuration
├── _layouts/
│   └── default.html            # Custom layout with header/nav/footer
├── assets/
│   └── css/
│       └── style.scss          # Custom Leiden University styling
├── index.md                    # Home page
├── syllabus/
│   └── index.md                # Syllabus with boot camp content + sidebar TOC
├── presentations/
│   └── index.md                # Presentations page (add PDFs here)
├── assignments/
│   └── index.md                # Assignments page
├── style-guide/
│   ├── index.md                # Style guide page
│   └── 22082025_Spring 2025_Leiden Koreastudies Thesis Style Guide.pdf
├── protocol/
│   ├── index.md                # Protocol page
│   └── BAKS Thesis Protocol_2025.pdf
├── readings/                   # Course readings
│   └── Mullaney_Rea_Where_Research_Begins.pdf
├── rubrics/                    # Assignment rubric PDFs
│   ├── Assignment 1_rubric_BAKS thesis.pdf
│   ├── Assignment 2_rubric_BAKS thesis.pdf
│   └── Assignment 3_rubric_BAKS thesis.pdf
├── BA-Eindwerkstuk_Syllabus_Spring2025.pdf  # Downloadable syllabus
├── README.md
└── .gitignore
```

---

## Key Course Information

### Weekly Schedule (Boot Camp)

| Week | Date | Topic |
|------|------|-------|
| 1 | Feb. 06 | Developing a Research Question and Identifying the Research Problem |
| 2 | Feb. 13 | Data and Sources – Generation, Collection, and FAIR Principles |
| 3 | Feb. 20 | Conducting a Literature Review |
| 4 | Feb. 27 | Analysis and Reporting – Empirical Strategies for Data Interpretation |

### Deadlines

| Assignment | Due Date |
|------------|----------|
| Assignment #1 (Revised Proposal) | March 13, 2026 |
| Assignment #2 (Preliminary Draft) | April 03, 2026 |
| Assignment #3 (Empirical Draft) | May 06, 2026 |
| Final Manuscript | June 01, 2026 |

### Evaluation Weights

- Participation: 10%
- Assignment #1: 20%
- Assignment #2: 35%
- Assignment #3: 35%

### Meeting Schedule

- Fridays, 09:15-11:00
- Location: Lipsius 2.05, Workgroup 103

---

## Maintenance Tasks

### Adding Presentation PDFs

After each lecture (weeks 1-4, plus week 6):

1. Add PDF to `presentations/` folder
2. Update `presentations/index.md` - replace "—" with link:
   ```markdown
   | 1 | Feb. 06 | Developing a Research Question... | [PDF](week01-research-question.pdf) |
   ```

### Updating Syllabus PDF

If the Word document is updated:
1. Open `27.02.2025_Eindwerkstuk-updated-scd.docx` in Word/Pages
2. Export as PDF
3. Replace `BA-Eindwerkstuk_Syllabus_Spring2025.pdf` in repo root
4. The docx file is gitignored and won't be pushed

### URL Structure

Pages use folder-based URLs:
- `/syllabus/` not `/syllabus.html`
- `/presentations/` not `/presentations.html`

### PDF Links

Use Jekyll's `relative_url` filter for PDF links:
```markdown
[Download PDF]({{ '/rubrics/Assignment 1_rubric_BAKS thesis.pdf' | relative_url }})
```

---

## Technical Notes

### Custom Theme Setup

The site uses Cayman theme with custom overrides:
- `_layouts/default.html` - Custom header with navigation
- `assets/css/style.scss` - Imports Cayman then overrides styles
- `.page-header { display: none !important; }` hides default Cayman header

### Sidebar TOC (Syllabus page)

The syllabus page uses a two-column layout with sticky sidebar:
- Uses `.page-layout` CSS grid
- TOC links use anchor IDs matching heading text
- Font: Source Sans Pro, 0.95rem

### Leiden University Colors

```css
--leiden-blue: #002147;
--leiden-gold: #c4a000;
```

### Troubleshooting

If site doesn't update after push:
1. Check Actions tab in GitHub for build errors
2. Verify Pages is enabled in Settings > Pages
3. Clear browser cache
4. Check SCSS syntax (empty front matter `---` required)

---

## Files Not in Version Control

See `.gitignore`:
- `.claude/` (Claude Code local settings)
- `.DS_Store` (macOS)
- `*.docx` (Word source documents)

---

## Brightspace Landing Page Text

The following text is used on the Brightspace workgroup landing page to direct students to the course website:

> **Course Website**
>
> The syllabus, due dates, and all resources you need for this course—including the style guide, thesis protocol, and assignment rubrics—are available on the course website:
>
> **https://scdenney.github.io/baks_thesis-seminar/**
>
> The website is designed to be easier to navigate than Brightspace. Please use it as your primary reference for course information throughout the semester.
>
> A PDF version of the syllabus is also available in the **Syllabus** folder in the navigation panel on the left.

---

## Related Resources

- [BA2 Digital Korea site](https://github.com/scdenney/ba2_digital-korea) - Design template
- [Chicago Manual of Style](https://www.chicagomanualofstyle.org/) - Citation reference
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [BA Final Paper Koreastudies Prospectus](https://studiegids.universiteitleiden.nl/en/courses/134317/ba-final-paper-koreastudies)
