# From tracing model transfer to predicting it

A talk on network analysis, scientific discovery, and the prediction of model transfer,
using the Grid Protocol Quarto / Reveal.js template from `MNoichl/ai4sci2026`.

The deck has a title slide, seven content slides, and references. On-screen bullets summarize
the supplied outline; the full passages are retained in speaker notes.

## Edit and preview

Edit `index.qmd` for slide content and `references.bib` for the bibliography.
The template controls typography, spacing, bullets, and automatic columns.
Use its `gp-dense` class for longer slides. The few content-specific rules
(author affiliations, the comparison table, and longer text measures) are at
the end of `gp-quarto.css`; avoid overriding all slide headings or lists.

```sh
quarto render index.qmd
quarto preview index.qmd
```

`index.html` and `index_files/` are generated output. To view the already rendered
deck without Quarto, serve the repository over HTTP:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then open <http://127.0.0.1:8000>. Use the arrow keys to advance through bullet
reveals and slides; press **S** for speaker notes.

## PDF export

With Playwright, pypdf, and Chrome installed:

```sh
python3 tools/export_pdf.py --mode slides --out export/model-transfer_slides.pdf
```

Add `--no-render` to use the existing HTML. Omit `--mode slides` for a page per
reveal step. Export files are ignored by Git. Jost and Newsreader are bundled locally, including their open font licenses.

## Citation details to resolve

- The supplied outline says “Wung et al. 2023”; the deck uses Wang et al. (2023),
  matching the supplied reference list.
- Karikó (2023) is retained as a footer citation; the outline did not supply its
  full bibliographic entry.
