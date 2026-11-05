# Saivana Quality Tracker

The website for the Saivana Quality Tracker: Dynamic Agencies inspection reports and our own DHU checks.

- Opens with a password. The data is stored locked (AES-256), and the page unlocks it in the browser.
- Nothing readable is stored in this repository. The locked data comes from the tracker's Google script.
- The website is read-only. Only the owner adds or changes reports and DHU sheets, and changes show here about a minute later.

## What the website shows

- **Overview** for the month chosen in the filters (it opens on the latest full month):
  - Headline figures with pieces checked.
  - Report cards: a score out of 100 and an A–F grade for each factory and buyer, with a table of where every point comes from.
  - Defects by type and department, how close each lot came to failing, week by week, factories and buyers, and measurements out of tolerance.
  - The **5 most important things**, each with the numbers from the reports as proof.
  - How to read the page.
- **DHU tracker** tab, for the month and factory chosen:
  - Stitching and finishing DHU, the stitching faults that reached finishing, finishing's own DHU and the pieces sent back.
  - Stitching lines, the styles letting most stitching faults through, where finishing defects come from, the quality chain up to Dynamic, and buyers.
  - The **5 most important things**, Claude's monthly review and how to read the DHU numbers.
- **Monthly PDF** and **DHU PDF** buttons that make printable reports.
- `vendor/` holds jsPDF and jsPDF-AutoTable (MIT licence), used to make the PDFs.
