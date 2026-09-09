# BAKS Thesis Seminar — Handoff

Read by `/sitrep` (start of session) and updated by `/finished` (end of session).
Newest entry at the top; don't rewrite history — append.

---

## 2026-02-28 (site built and populated; dated from the file's own 'Feb 2026' headings — this content was moved from CLAUDE.md on 2026-09-09)

### Initial Setup (Feb 2026)

1. **Created Jekyll site** matching the BA2 Digital Korea site design
   - Custom layout (`_layouts/default.html`) with Leiden University branding
   - Custom SCSS styling (`assets/css/style.scss`) with Leiden colors (blue #002147, gold #c4a000)
   - Uses Cayman theme as base with custom overrides

2. **Fixed folder naming issue**
   - Renamed `rubrics ` → `rubrics` (removed trailing space)

3. **Created site pages** using folder-based structure:
   - `index.md` - Homepage with overview, schedule, deadlines
   - `syllabus/index.md` - Full syllabus with boot camp content (weeks 1-4) and sidebar TOC
   - `presentations/index.md` - Lecture slides (weeks 1-4 plus week 6 pre-recorded lecture)
   - `assignments/index.md` - Assignment details with rubric links
   - `style-guide/index.md` - Formatting and citation guidelines
   - `protocol/index.md` - Thesis expectations and assessment

4. **Created syllabus PDF** from Word document
   - Manually converted `27.02.2025_Eindwerkstuk-updated-scd.docx` to PDF
   - Saved as `BA-Eindwerkstuk_Syllabus_Spring2025.pdf`
   - Added download link on homepage and syllabus page

### Content Updates (Feb 2026)

1. **Syllabus page** - Added comprehensive boot camp content for weeks 1-4:
   - Week 1: Developing a Research Question and Identifying the Research Problem
   - Week 2: Data and Sources – Generation, Collection, and FAIR Principles
   - Week 3: Conducting a Literature Review
   - Week 4: Analysis and Reporting – Empirical Strategies for Data Interpretation
   - Each week includes objectives, readings, class plan, and exercises
   - Added sticky sidebar table of contents

2. **Weekly schedule formatting**:
   - Assignment due dates use dash (—) instead of week number
   - No extra text after assignment dates (removed "No class – plan meeting with supervisor")
   - Week numbers only for actual class sessions

3. **Presentations page** - Added Week 6 (Mar. 20) pre-recorded lecture reviewing weeks 1-4

4. **Protocol and Style Guide pages** - Added intro text noting pages provide basic overview; download PDF for complete information

5. **Fixed links**:
   - BA Final Paper Koreastudies Prospectus: https://studiegids.universiteitleiden.nl/en/courses/134317/ba-final-paper-koreastudies
   - Plagiarism regulations: https://www.organisatiegids.universiteitleiden.nl/en/regulations/general/plagiarism

6. **CSS updates** - Fixed TOC sidebar font to be consistent with site font (Source Sans Pro, 0.95rem)

7. **Brightspace submission** - Added note that all assignments are due by 23:59 via Brightspace (on both Assignments and Syllabus pages)

8. **Readings folder** - Added `readings/` folder with course textbook PDF (Mullaney & Rea, *Where Research Begins*); linked in Week 1 syllabus section

9. **Folder consolidation** - Merged duplicate folders:
   - `style_guide/` (PDFs) + `style-guide/` (page) → `style-guide/` (now contains both)
   - `thesis_protocol/` (PDF) + `protocol/` (page) → `protocol/` (now contains both)
   - Updated PDF links in markdown files to new locations

10. **Syllabus page cleanup** - Removed redundant course information (already on homepage); renamed section to "About This Seminar" with expanded description of thesis expectations and seminar structure

11. **Date correction** - Fixed all course dates from 2025 to 2026 (Spring semester of AY2025-2026)
