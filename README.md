# Youden Index Paired Bootstrap Calculator

A browser-based calculator for comparing the Youden index between two paired biomarkers using patient-level paired bootstrap resampling.

## Features

This tool supports Excel (`.xlsx`, `.xls`) and CSV files with at least three columns:

- outcome
- marker 1
- marker 2

It calculates:

- optimal cutoff
- sensitivity
- specificity
- accuracy
- Youden index
- observed Youden index difference
- paired bootstrap 95% confidence interval
- two-sided bootstrap p value

## Recommended settings for Jason's current analysis

- Positive outcome value: `0`
- Prediction direction: `Lower marker value predicts positive`
- Cutoff method: `Re-optimize cutoff in each bootstrap sample`
- Bootstrap iterations: `10000`
- Random seed: `2026`

## GitHub Pages deployment

1. Create a new GitHub repository.
2. Upload `index.html`, `README.md`, and `.nojekyll` to the repository root.
3. Go to repository **Settings** → **Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch: `main`; folder: `/root`.
6. Save.

The site will be published at:

`https://<your-github-username>.github.io/<repository-name>/`

## Privacy note

This is a static webpage. Calculations are performed in the user's browser. There is no backend server. For sensitive clinical data, remove patient identifiers before analysis.
