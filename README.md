# State Sponsorship and Terrorist Organization Lethality (1998–2005)

Econometrics research project examining the relationship between state sponsorship and recorded civilian fatalities among organizations in the Big Allied and Dangerous (BAAD I) dataset.

## Research question

What is the relationship between state sponsorship and the lethality of terrorist organizations from 1998 to 2005?

## Dataset and approach

The BAAD analytical sample includes **395 organizations** (**32 sponsored**, **363 nonsponsored**). Supplementary NAG active- and de facto-support records were linked for exploratory support-type comparisons; **17 of 32 sponsored organizations** were linked. Methods include descriptive analysis, log-OLS regression with HC3 robust standard errors, propensity-score matching, PPML, logistic regression, and sensitivity checks.

## Selected findings

- **75.0%** of sponsored organizations and **36.1%** of nonsponsored organizations recorded at least one fatality.
- Unadjusted log-OLS sponsorship coefficient: **1.645** (HC3 p < 0.001).
- Fully adjusted log-OLS sponsorship coefficient: **0.089** (HC3 p = 0.805).
- Primary matching: **30 pairs**, average recorded-fatality difference **+25.67** (p = 0.337).
- Capacity-adjusted matching: **26 pairs**, average recorded-fatality difference **−122.23** (p = 0.385).

These estimates are observational associations, not identified causal effects. Matching balance is imperfect and organizational-capacity controls could be post-treatment variables.

## Files

- [`analysis/ECO4422_Project.Rmd`](analysis/ECO4422_Project.Rmd): original finalized R Markdown analysis **unchanged**.
- [`analysis/ECO4422_Project.html`](analysis/ECO4422_Project.html): rendered analysis output.
- [`report/Part3_Report.pdf`](report/Part3_Report.pdf): Part 3 report.
- [`report/Part3_Report.tex`](report/Part3_Report.tex): editable LaTeX source.
- [`figures/figure1_raw_fatalities.pdf`](figures/figure1_raw_fatalities.pdf): raw fatality figure.
- [`data/source/`](data/source/): original BAAD `.sav` and both NAG support `.csv` data files.

## Reproducibility notes

The three original source datasets are included under `data/source/`. Their dimensions correspond to the analysis: BAAD has **395 organizations and 19 variables** (as recorded in the finalized R Markdown), while each NAG support CSV has **6,910 observations** (15 active-support variables; 14 de facto-support variables). The source files have not been altered; only their downloaded filenames have been simplified.

The finalized `.Rmd` is intentionally **unchanged** and still references absolute macOS paths for the original data. To reproduce on another computer, configure the input paths in a local copy to point to `data/source/`. The notebook creates an `outputs/` directory for generated artifacts. The bundled rendered HTML is a snapshot of the finalized analysis.

**Public-data rights:** Before publishing this repository publicly, confirm that the licenses or terms for BAAD and the NAG data permit redistribution. If not, remove `data/source/` from the public GitHub repository and provide data acquisition instructions instead. The original sources were supplied for the course submission; their redistribution rights were not established.

The Part 3 PDF currently contains unresolved bibliography citation markers; the `.bib` file from the Overleaf project was not provided.

## Authorship

Katelyn McCullough — ECO 4422 Econometrics, Florida Polytechnic University (2026).
