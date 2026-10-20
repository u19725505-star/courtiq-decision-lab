# CourtIQ — The Decision Lab

**An interactive basketball analytics experience** investigating whether shot context and defensive pressure improve shot-make prediction on held-out games.

## Live judge experience

- **Live demo:** https://u19725505-star.github.io/courtiq-decision-lab/
- **Source repository:** https://github.com/u19725505-star/courtiq-decision-lab
- **Notebook folder:** [Notebook](https://github.com/u19725505-star/courtiq-decision-lab/tree/main/Notebook)
- **Figures:** [figures/](https://github.com/u19725505-star/courtiq-decision-lab/tree/main/figures)
- **Tables and source data:** [tables/](https://github.com/u19725505-star/courtiq-decision-lab/tree/main/tables)

The experience includes a basketball opening reel, a seven-step narrated judge walkthrough, animated model comparison, saved metric results, a rotatable source-coordinate explorer, a game-level robustness summary, and an explicit limitations review. Browser speech availability depends on the judge's device; all key points are also presented on screen.

## Reported research snapshot

| Measure | Reported result |
|---|---:|
| Shot records in engineered dataset | 1,459 |
| Game clusters | 10 |
| Saved out-of-fold model probability streams | 5 |
| Shot-ID join coverage | 100% |
| Best ROC-AUC | 0.6549 — contest-level model |
| Best Brier score | 0.2237 — contest-level model |
| Highest average precision | 0.6172 — both defensive features |
| Paired game-cluster bootstrap AUC gain vs baseline | +0.0648 |
| Reported 95% interval for AUC gain | [0.0383, 0.0874] |

The contest-level model has the strongest reported ROC-AUC and Brier score. The model with both defensive features has the highest average precision and slightly better log loss. These metrics answer different questions; no single model wins every metric.

## Spatial-data provenance and limits

The repository includes `data/court_shots.json`, parsed from `tables/source_shots_raw.csv`. It contains **1,433 parseable source coordinate pairs across 10 games**. The interactive explorer plots those source values, normalizing them for display. Height is a visual encoding of shot distance, not measured ball trajectory.

**Important:** the source coordinate axis convention, orientation, and court calibration have not been independently verified. The explorer is therefore a source-coordinate visualization, not a verified regulation-court shot chart. Do not infer exact court zones or coaching prescriptions from its geometry until that validation is complete.

## Interpretation and limitations

- These are predictive associations, not causal proof and not evidence of demonstrated game-winning impact.
- The reported robustness check has only 10 game clusters; uncertainty intervals may be unstable.
- Results need independent evaluation across more games and, ideally, teams or seasons not represented in model development.
- Further work should verify coordinate semantics, evaluate calibration and subgroup performance, and test whether the information improves real decisions prospectively.
- This prototype is a research demonstration, not a live coaching or player-evaluation system.

## Judge walkthrough

1. Open the live demo and select **Judges Entrance**.
2. Follow the seven chapters in order: research questions, data, spatial explorer, model evidence, robustness, limitations, and final play.
3. Use the layer controls and drag/rotate controls in the spatial explorer.
4. Compare ROC-AUC, Brier score, average precision, and log loss rather than relying on a single headline number.
5. Finish by reviewing the validation limits and future work.

If narration is unavailable, use the visible chapter text and the Next/Back controls. On mobile, rotate to landscape for the spatial visualization if needed.
