# Saivana Quality Tracker

The website for the Saivana Quality Tracker: Dynamic Agencies inspection reports, overview and report list.

- Opens with a password. The reports are stored locked (AES-256), and the page unlocks them in the browser.
- New reports appear about a minute after they are saved in the tracker.
- The locked data comes from the tracker's Google script; nothing readable is stored in this repository.

## What the website shows

- Overview with early warnings (what is getting worse), report cards with an A–F grade for each factory and buyer, and Claude's analysis of each report.
- A **DHU tracker** tab: our own 100% checks (stitching, finishing, embroidery, cutting): DHU by factory and line, where finishing defects come from, the quality chain up to Dynamic, buyers, and Claude's monthly review. DHU sheets are uploaded in the tracker in Claude.
- A **Monthly PDF** button that makes a printable report for the month chosen in the filters.
- Reports are added, edited and deleted in the Saivana Quality Tracker in Claude; the "Add a report" tab links there.
- `vendor/` holds jsPDF and jsPDF-AutoTable (MIT licence), used to make the PDF.
