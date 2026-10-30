# hs4002-dalmation-2026

HS4002 Team Research Project, Team Dalmation: Yu Xin, Shi Han (Joyce), Janelle, Audris

**Research question:** To what extent does the association between socioeconomic status and
relationship stability vary across racial groups in the US?

**Dataset:** How Couples Meet and Stay Together 2017–2020–2022 combined dataset
(Rosenfeld, Thomas & Hausen, 2023).

> Our first analysis (Presentation #1) used HCMST 2009 by mistake. It is kept in
> [`archive/hcmst2009/`](archive/hcmst2009/) and as the git tag `v1-hcmst2009`.

## Getting the data

We use the HCMST 2017–2020–2022 combined dataset, public version 2.2 (Stata format),
downloaded from <https://data.stanford.edu/hcmst2017> as
`HCMST 2017 to 2022 small public version 2.2.dta` on 30 October 2026.

The file is already in this repository as
`data/raw/HCMST_2017_to_2022_small_public_version_2.2.dta` (4MB). Stanford's data use agreement
allows sharing it free of charge, provided it is not used to identify individuals and is cited.
If you download it yourself, rename it to that file name and place it in `data/raw/`.

The codebook (v2.2) and user's guide (v2.3) are in `docs/`.

**Citation:** Rosenfeld, Michael J., Reuben J. Thomas, and Sonia Hausen. 2023. How Couples Meet and
Stay Together 2017-2020-2022 combined dataset. [Computer files]. Stanford, CA: Stanford University
Libraries. https://data.stanford.edu/hcmst2017

## Run order

Work in progress. Notebooks will run in this order:

1. `code/01_clean.ipynb`: keep partnered respondents; income, education and earnings variables
2. `code/02_relationship_stability.ipynb`: track each 2017 relationship to 2020 and 2022; breakups, partner deaths, attrition, panel set-up
3. `code/03_race.ipynb`: respondent race, partner race, same-race flag
4. `code/04_analysis.ipynb`: logistic regression models and charts

## Folders

- `code/`: notebooks
- `data/raw/`: the data as downloaded, never edited by hand
- `data/processed/`: cleaned data produced by the notebooks
- `docs/`: codebook and user's guide
- `output/tables/`, `output/figures/`: results
- `slides/`: presentation slides (`presentation1.pdf` = Presentation #1, 7 Oct 2026; its results
  come from HCMST 2009, see `archive/hcmst2009/`)
- `archive/hcmst2009/`: earlier analysis on HCMST 2009
