# Statistical Programming Practical (Oxford)

This repository contains material for the MSc Statistical Programming Practical 2024 at the University of Oxford. It includes the R Markdown source, LaTeX output, data files, and supporting figures used to complete the assessed practical (project code P468).

## Repository structure

- `P468.Rnw` – The Sweave/LaTeX source for the final report.
- `P468.tex` / `P468.pdf` – Compiled LaTeX and PDF versions of the report.
- `AA-NNAA-FP.csv`, `Average-prices-2024-07.csv`, `series-201024.csv` – Data files referenced throughout the analysis.
- `figure/` – Graphics generated from the R code.
- `Assessed_practical.Rproj` – RStudio project file for reproducing the analysis.
- `MSc Statistical Programming Practical 2024.pdf` – Coursework brief and guidelines.

## Getting started

1. Open `Assessed_practical.Rproj` in RStudio.
2. Ensure the required R packages for Sweave/knitr and plotting are installed (e.g. `knitr`, `ggplot2`, `dplyr`).
3. Knit `P468.Rnw` to produce updated `P468.tex` and `P468.pdf` outputs.

## Reproducing the report

To rebuild the report from the command line, you can run the following in R:

```r
R CMD Sweave P468.Rnw
pdflatex P468.tex
```

Running `pdflatex` twice helps resolve cross-references in the document.

## License

All course material is provided for educational use as part of the MSc Statistical Programming Practical. Please contact the course convenors if you plan to redistribute or adapt any part of this repository.
