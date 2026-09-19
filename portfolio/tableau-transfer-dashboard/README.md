# Context-Aware Player Transfer Performance Dashboard

Interactive Tableau dashboard built from the player-transfer stage of my MSc Computer Science football-modelling project.

## Question

How does a player's performance change after moving clubs, and can a context-aware model predict that change better than simply carrying forward the player's previous-season performance?

## Held-out result

Across **255 transferred players** and **43 player performance measures**, the context-aware model reduced scaled prediction error by **7.79%** relative to the carry-forward baseline.

| Evaluation | Scaled error |
| --- | ---: |
| Carry-forward | 0.5426 |
| Context-aware model | 0.5003 |
| Improvement | **7.79%** |

## What the dashboard does

- Select an individual transferred player.
- View the player's source and destination club.
- Select an interpretable per-90 performance metric.
- Compare carry-forward, context-aware prediction and observed post-transfer performance.
- See where contextual modelling improved prediction accuracy and where carry-forward performed better.

The dashboard presents eight accessible metrics for visual exploration. The **7.79%** headline evaluation is calculated on the locked held-out cohort across all **43** modelled measures, rather than only the eight displayed metrics.

## Files

- [`Context-Aware-Player-Transfer-Performance.twb`](Context-Aware-Player-Transfer-Performance.twb) — Tableau workbook.
- [`tableau_transfer_dashboard.csv`](tableau_transfer_dashboard.csv) — public-safe dashboard dataset used by the workbook.

The workbook's data connection has been normalised to the CSV in this same folder for portability. If Tableau prompts for a data source after download, select `tableau_transfer_dashboard.csv`.

## Data / research boundary

This portfolio export contains only dashboard-level derived values. The original research database, private fitted model artefacts and internal pipeline outputs are not included.

## Tools

Tableau, Python, SQL, pandas and statistical modelling.
