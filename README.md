# CourtIQ — The Decision Lab

**An interactive basketball analytics experience** exploring shot context, defensive pressure, out-of-fold model evidence, game-level robustness, and spatial analytics limitations.

## Live judge experience

Open the live experience: https://u19725505-star.github.io/courtiq-decision-lab/

The site includes:
- A basketball opening reel and sports-broadcast-inspired presentation.
- A browser-based AI voice narrator with play, pause, and stop controls. Voice availability and perceived gender depend on voices installed on the visitor's browser/device.
- A research-question scoreboard with explicit questions and testable hypotheses.
- An animated model leaderboard and full saved metric table.
- A rotatable 3D-style court schematic with illustrative distance/pressure layers.
- A guided explanation of evaluation, game-level robustness, and research limitations.

## Current reported research snapshot

- 1,459 shot records across 10 games
- Five saved out-of-fold model probability streams
- Best reported ROC-AUC: 0.6549 (contest-level model)
- Best reported Brier score: 0.2237 (contest-level model)
- Reported OOF shot-ID join coverage: 100%
- Reported paired game-cluster bootstrap AUC gain: +0.0648, 95% interval [0.0383, 0.0874]

## Spatial-data honesty

The current engineered dataset does **not** contain verified court x/y coordinates. The court view is an interactive schematic intended to explain the spatial analytics concept; its markers are illustrative, not actual shot locations. Real shot mapping requires verified coordinates and a documented court-coordinate convention.

## Interpretation and limitations

The current results are predictive evidence, not causal proof and not a claim of demonstrated game-winning impact. Only 10 game clusters are represented in the reported robustness audit, so uncertainty estimates may be unstable. Independent validation on more games is necessary before decision-support claims.

## Research source

- [Repository](https://github.com/u19725505-star/courtiq-decision-lab)
- [Notebook folder](https://github.com/u19725505-star/courtiq-decision-lab/tree/main/Notebook)
- [Figures folder](https://github.com/u19725505-star/courtiq-decision-lab/tree/main/figures)
- [Tables folder](https://github.com/u19725505-star/courtiq-decision-lab/tree/main/tables)
