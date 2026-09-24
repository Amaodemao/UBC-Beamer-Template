# UBC-Beamer-Template
This is a beamer template adapted for the University of British Columbia (UBC).

## Build

Compile from the repository root with TeX Live and XeLaTeX:

```sh
latexmk -xelatex -interaction=nonstopmode -halt-on-error -outdir=build beamerUBC.tex
```

The result is `build/beamerUBC.pdf`. On Overleaf, choose `beamerUBC.tex` as
the main document and XeLaTeX as the compiler.

## Files

- `beamerUBC.tex`: packages, presentation metadata and document entry point.
- `slides/demo.tex`: the example slides; replace these with your own content.
- `beamerthemeubc.sty`: page layout, cover, headers, footers and existing commands.
- `ubccolor.sty`: official UBC blues plus neutral and semantic colours.
- `assets/ubc/`: official vector logos and the Vancouver campus photograph.
- `assets/ubc/SOURCES.md`: source URLs and asset notes.
- `bibliography.bib`: example references.

The original CUHK directory and `assets/legacy-cuhk/` are local reference
copies excluded from Git. The UBC theme does not depend on either directory.

## Visual Style

The cover uses UBC Blue (`#002145`), the official white full signature,
and left-aligned title, author, affiliation and date. Uncomment the
`\titlebackground*` line for the optional campus-photo cover.
Content slides use a white background, a blue crest, dark text and neutral
blocks. The page is 20 cm by 11.25 cm (16:9).

The existing fonts, section transitions, automatic subtitles, frame counting
and public commands remain in place. The theme name is now `ubc`;
legacy `sintef...` colour aliases remain available in `ubccolor.sty`.

## Acknowledgments & License
This template is modified from [CUHK-Beamer-Template](https://www.overleaf.com/latex/templates/xiang-gang-zhong-wen-da-xue-zhong-wen-mo-ban-cuhk-beamer-template/bpgghjpjkqxw) by Richard Fury.

Modifications by [Haonan Bai] (2026) are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
