# Fontmark

Preview your text in every font on your machine, shortlist favourites, and export or compare them — a [wordmark.it](https://wordmark.it)-style type tool in a single HTML file.

**Live site:** https://tanvirahmed1732.github.io/fontmark/

## Features

- Instant detection of installed system fonts (canvas probing, works in every browser)
- **Load all installed fonts** via the Local Font Access API (Chrome/Edge) — one card per installed style
- Add any installed font by its exact name; drag-and-drop `.ttf/.otf/.woff/.woff2` files to preview uninstalled fonts
- Shortlist, isolate, and drag-to-rank favourites; click a shortlisted font to jump to its card in the grid
- Size slider, case toggle, negative (white-on-black) mode, custom text colour, search
- Collections with tags (saved in the browser), PNG specimen-sheet export, copy-as-text list, side-by-side compare view
- Zoom any font (from its card, its shortlist row, or its Compare tile) into a popup sized to fit on opening; the size then stays put while you type (the text wraps, and scrolls if it outgrows the popup) and changes only with the size slider or **Fit**. It comes with **swash controls**: switch OpenType features (swash, stylistic alternates and sets, ligatures) on or off per font, click a letter to pick one of its alternates, and attach standalone tail strokes after a letter. Choices are remembered per font and carry into Compare.

Swash controls read the font file itself, so they work for uploaded fonts and after **Load all installed fonts** (the canvas-detected set is known by name only). The font parser ([opentype.js](https://github.com/opentypejs/opentype.js)) is fetched from cdnjs the first time the controls are used; `.woff2` uploads can't be read.

## Files

- `index.html` — the deployed page (full HTML document)
- `fontmark.html` — the app source as page content only (no `<html>/<head>/<body>` wrapper; used as a Claude Artifact)

After editing `fontmark.html`, rebuild `index.html` by re-wrapping it (same head/body shell, with the leading `<title>` line dropped).
