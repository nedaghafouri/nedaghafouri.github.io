# Neda Ghafouri — personal website

A single-page academic homepage. No build step and no Jekyll, so GitHub Pages serves the files as they are.

```
index.html                  the whole site (HTML + CSS + a few lines of JS)
assets/neda-photo.jpg       portrait
assets/figures/             one figure per paper (click to enlarge on the site)
files/                      CV and paper PDFs
.nojekyll                   tells GitHub Pages to skip Jekyll
```

## Where it lives

This repository is `nedaghafouri/nedaghafouri.github.io`, so GitHub Pages serves it at **https://nedaghafouri.github.io** from the `main` branch root. Any change pushed to `main` goes live within a minute or two.

## Updating the site

Everything is in `index.html`. Search for the comment markers:

- **News**: find `NEWS` and copy one `<tr>` row to the top of the table.
- **A new paper**: find `PUBLICATIONS` and copy a whole `<li id="p-...">…</li>` block. Edit the venue badge (`abbr`), figure, title, authors, venue line, one-line highlight, the `ABS` summary and the link buttons. Give the copied block, its `abstract` box and its `aria-controls` a new id.
- **Figures** live in `assets/figures/`. Clicking a figure opens it full size.
- **Research areas**: the bulleted list in the about section links each paper by its `#p-...` id.
- **Experience and education**: copy one `<li>` in the matching list; the date goes in the `when` badge.
- **CV**: replace `files/Neda_Ghafouri_CV.pdf` with a new file of the same name.
- Change "Last updated" in the footer when you edit.
