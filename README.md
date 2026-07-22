# Fontmark

Preview your text in every font on your machine, shortlist favourites, and export or compare them — a [wordmark.it](https://wordmark.it)-style type tool in a single HTML file.

**Live site:** https://tanvirahmed1732.github.io/fontmark/

## Features

- Instant detection of installed system fonts (canvas probing, works in every browser)
- **Load all installed fonts** via the Local Font Access API (Chrome/Edge) — one card per installed style
- Add any installed font by its exact name; drag-and-drop `.ttf/.otf/.woff/.woff2` files to preview uninstalled fonts
- Shortlist, isolate, and drag-to-rank favourites
- Size slider, case toggle, negative (white-on-black) mode, custom text colour, search
- Collections with tags (saved in the browser), PNG specimen-sheet export, copy-as-text list, side-by-side compare view

## Files

- `index.html` — the deployed page (full HTML document)
- `fontmark.html` — the app source as page content only (no `<html>/<head>/<body>` wrapper; used as a Claude Artifact)

After editing `fontmark.html`, rebuild `index.html` by re-wrapping it (same head/body shell, with the leading `<title>` line dropped).
