# JUMPCP_Production_Analysis — Archive Summary

- Repo: https://github.com/srijitseal/JUMPCP_Production_Analysis
- Author: Srijit Seal
- Period: Dec 2025 – Jan 2026
- Status: Superseded by jump_production

## Contents

Marimo notebooks organized into four analysis modules:

- `01_mAP/` — Activity mAP on harmony profiles and a cell-count-only (X_623) baseline. Params: batch_size=20000, null_size=20000, fdr=0.1.
- `02_analyse_map/` — Exploratory analysis of activity results. Edge-well effects on AP (no significant effect found). Compound- and profile-level mAP vs cell count (weak negative correlation). AP distribution by source and well position (no plate position trends).
- `03_global_organisation/` — Chemical space visualization using RDKit physicochemical descriptors, PCA, and pairwise distance distributions.
- `04_map_datasets/` — Consistency mAP (target retrieval) for three annotation sources: ChEMBL targets, MoA, and ToxCast. Median-aggregated compound profiles, multilabel AP, volcano plots.

## What moved to jump_production

Activity mAP and all three consistency analyses are now reproduced in [jump_production](https://github.com/broadinstitute/jump_production) via copairs-runner, expanded to 9 annotation sources across multiple datasets and preprocessings.

Not yet reproduced: the cell-count-only activity baseline, the plate-effect and cell-count exploratory analysis (findings were negative).
