# Cisco 800-150 Study Lab

This is a dependency-free static study site. `questions.json` is the permanent
data source; the browser application never reads or parses the PDF.

To run locally from this folder:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000` in a browser.

The one-time PDF extractor is kept in `work/extract_questions.py`. Only run it
when replacing or correcting the source PDF. The 23 drag-and-drop questions are
intentionally marked `needsReview: true` because their PDF tables showed no
yellow-highlighted answer key; they are not included in scoring.
