# hs4002-dalmation-2026

HS4002 Team Research Project, Team Dalmation: Yu Xin, Shi Han (Joyce), Janelle, Audris

**Research question:** To what extent does the association between socioeconomic status and
relationship stability vary across racial groups in the US?

**Dataset:** How Couples Meet and Stay Together 2017–2020–2022 combined dataset
(Rosenfeld, Thomas & Hausen, 2023).

> Our first analysis (Presentation #1) used HCMST 2009 by mistake. It is kept in
> [`archive/hcmst2009/`](archive/hcmst2009/) and as the git tag `v1-hcmst2009`.

## Getting the data

1. Download the Stata (`.dta`) combined dataset from <https://data.stanford.edu/hcmst2017>.
2. Put it in `data/raw/`. Raw data is not committed (see `.gitignore`).

## Run order

Work in progress. Notebooks will run in this order:

1. `code/01_clean.ipynb`: load raw data, select and clean variables
2. `code/02_outcome.ipynb`: relationship stability outcome
3. `code/03_race.ipynb`: respondent race, partner race, same-race flag
4. `code/04_models.ipynb`: logistic regression models and charts

## Folders

- `code/`: notebooks
- `data/raw/`: raw data (not committed)
- `data/processed/`: cleaned data produced by the notebooks
- `output/tables/`, `output/figures/`: results
- `archive/hcmst2009/`: earlier analysis on HCMST 2009
