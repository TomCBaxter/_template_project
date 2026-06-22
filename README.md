 # Project Template

This repository is organized around a simple research workflow:

1. Raw or intermediate inputs live in `data/`.
2. Reusable logic goes in `src/`.
3. Analysis work can be explored in `notebooks/`.
4. Figures, writing, and final paper outputs live in `proj/`.
5. Utility scripts belong in `scripts/`.

## Directory Structure

```text
.
├── README.md
├── data/
├── notebooks/
│   └── SpecificFiguresAnalysis.ipynb
├── proj/
│   ├── notes/
│   └── tex/
│       ├── bib.bib
│       └── main.tex
├── scripts/
└── src/
	├── analysis/
	└── core/
```

## Workflow

The usual workflow is to keep data preparation and reusable code separated from the presentation layer. Start with files in `data/`, develop analysis helpers in `src/core/` and `src/analysis/`, then use `notebooks/` for interactive inspection or figure generation. Once results are ready, move the writing and LaTeX build process into `proj/tex/`, while any repeatable command-line steps can go into `scripts/`.

`proj/tex/` is the output and manuscript area. Files such as `main.aux`, `main.bbl`, `main.blg`, `main.log`, `main.out`, `main.pdf`, and `main.synctex.gz` are generated during compilation and do not usually need to be edited by hand.

