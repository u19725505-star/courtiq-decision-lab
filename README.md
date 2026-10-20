# CourtIQ — The Decision Lab

**An evidence-driven basketball analytics experience exploring shot quality, defensive pressure, out-of-fold model evaluation, and game-level robustness.**

## Judge experience

The interactive judge walkthrough lives in [`index.html`](./index.html). It opens with a basketball video reel and an **Enter the Lab** button, then guides reviewers through the research question, dataset, evaluation method, model leaderboard, shot-intelligence concept, robustness evidence, limitations, and next steps.

If GitHub Pages is enabled for this repository's `main` branch with the repository root as the publishing source, the site should be available at:

https://u19725505-star.github.io/courtiq-decision-lab/

## Current reported research snapshot

- 1,459 shot records across 10 games
- Five saved out-of-fold model probability streams
- Best reported ROC-AUC: 0.6549 (contest-level model)
- Best reported Brier score: 0.2237 (contest-level model)
- Reported OOF shot-ID join coverage: 100%

## Important limitations

The current engineered dataset does not contain genuine court x/y coordinates. The website labels schematic court illustrations as illustrative rather than observed shot locations. Current results are predictive evidence on a small set of games, not causal proof or a claim of demonstrated game-winning impact. Independent external-game validation remains necessary.

## Research source

- [Repository](https://github.com/u19725505-star/courtiq-decision-lab)
- [Project files](https://github.com/u19725505-star/courtiq-decision-lab/tree/main)
