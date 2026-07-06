# Chapter alignment: Instructor book ↔ main book

This file tracks how the **instructor resources** (this repo,
`BB512_Instructor`) line up with the **student book**
(`jonesor/BB512_Book`). The instructor book exists to support teachers
running the activities in the main book, so every student activity should
have a matching instructor chapter, in the same order.

Keep this table in step whenever a chapter is added to either book. Chapter
order is pinned in `_bookdown.yml` (`rmd_files:`) to match the main book.

_Last reconciled: 2026-07-06 against `BB512_Book@master`._

## Alignment table

| Main book chapter | Instructor file | Status |
|---|---|---|
| 2 The Blind Watchmaker | `1_01_BlindWatchmaker.Rmd` | ✅ matched |
| 3 Bug hunt camouflage (NetLogo) | `1_02_BugHuntCamouflage.Rmd` | ✅ matched |
| 4 Geometric growth | `2_02_GeometricGrowth.Rmd` | ✅ matched |
| 5 Estimating Population Growth Rate | `2_03_EstimatingLambda.Rmd` | ✅ matched |
| 6 Stochastic population growth | `2_04_StochasticGrowth.Rmd` | ✅ matched |
| 7 Basic logistic population growth | `2_05_BasicLogisticGrowth.Rmd` | ✅ matched |
| 8 Deeper into Logistic Growth | `2_06_DeeperIntoLogistic.Rmd` | ✅ matched |
| 9 Life tables and survivorship types | `2_07_LifeTables.Rmd` | ✅ matched |
| 10 Matrix population modelling | `2_07.5_matrixModels.Rmd` | ✅ matched |
| 11 Pre- and Post-reproduction census | `2_07.55_prePostBreeding.Rmd` | ✅ matched |
| 12 Life Table Response Experiments | `2_07.6_LTRE.Rmd` | ✅ matched |
| 13 How many eggs should a bird lay? | `2_08_HowManyEggs.Rmd` | ✅ matched |
| 14 Trade-offs and the declining force of selection | `2_09_TradeOffsForceOfSelection.Rmd` | ✅ matched |
| 15 Matrix Population Models (MPMs): Projection and Simulation | `2_10_MPMProjectionSimulation.Rmd` | 🆕 added (draft) |
| 16 Hardy-Weinberg equilibrium | `3_01_HardyWeinberg.Rmd` | ✅ matched |
| 17 The Gene Pool Model | `3_01.5_GenePool.Rmd` | ✅ matched |
| 18 Neutral or Adaptive Evolution in Humans | `3_02_NeutralOrAdaptiveEvolution.Rmd` | ✅ matched |
| 19 Heritability from a linear regression | `3_03_Heritability.Rmd` | ✅ matched |
| 20 Lotka-Volterra competition | `4_01_LotkaVolterraCompetition.Rmd` | ✅ matched |
| 21 Lotka-Volterra predator-prey dynamics | `4_02_LotkaVolterraPredatorPrey.Rmd` | ✅ matched |
| 22 Continuous-time Lotka-Volterra Predator-Prey Model in R | `4_03_LVPredatorPreyContinuousTime.Rmd` | 🆕 added (draft) |
| 23 Discrete-time Lotka-Volterra Predator-Prey Model in R | `4_04_LVPredatorPreyDiscreteTime.Rmd` | 🆕 added (draft) |
| 24 Game theory: Hawks and doves | `5_01_HawkDoveCardGame.Rmd` | ✅ matched |
| 25 Solutions and "take-home" messages | _(n/a — student-facing solutions)_ | ➖ no instructor chapter needed |
| 26 Results of the hawk-dove games | _(n/a — student-facing solutions)_ | ➖ no instructor chapter needed |
| 27 Exponential growth in detail | `7_01_LambdaAndR.Rmd` | ✅ matched |
| 28 The legend of Ambalappuzha | `7_02_Ambalapuzha.Rmd` | ✅ matched |
| 29 From population biology to fitness | `7_03_FromPopulationToEvolution.Rmd` | ✅ matched |
| 30 From plain English to a matrix model | `7_04_MatrixFromEnglish.Rmd` | 🆕 added (draft) |
| 31 Continuous traits from discrete genes | `7_05_DiscreteGenes.Rmd` | 🆕 added (draft) |
| 32 Building a phylogenetic tree | `7_06_Phylogeny.Rmd` | 🆕 added (draft) |

## Changes made in this pass (2026-07-06)

**New instructor chapters** drafted for the six main-book activities that
previously had no instructor support (marked 🆕 above). Each follows the
existing instructor format (Introduction → Learning Outcomes → Activity
Overview → Instructions for Facilitating → Questions & Model Answers →
Teaching Tips → Common Pitfalls) and is a **draft for review**.

**Chapter order pinned.** Added an explicit `rmd_files:` list to
`_bookdown.yml`. Previously bookdown merged chapters in filename
(string-sort) order, which put some chapters out of sequence relative to
the main book — e.g. `2_07.5`/`2_07.55` sorted *before* `2_07_LifeTables`,
and `3_01.5_GenePool` sorted *before* `3_01_HardyWeinberg`. The explicit
list restores the main-book order without renaming files.

**Title / spelling alignment** (instructor headings matched to the
student book):

| File | Was | Now |
|---|---|---|
| `1_02_BugHuntCamouflage.Rmd` | Bug **H**unt **C**amouflage (NetLogo) | Bug **h**unt **c**amouflage (NetLogo) |
| `2_06_DeeperIntoLogistic.Rmd` | Deeper into **l**ogistic **g**rowth | Deeper into **L**ogistic **G**rowth |
| `2_07_LifeTables.Rmd` | **L**ife **T**ables and **S**urvivorship **T**ypes | **L**ife **t**ables and **s**urvivorship **t**ypes |
| `2_09_TradeOffsForceOfSelection.Rmd` | …the **D**eclining **F**orce of **S**election | …the **d**eclining **f**orce of **s**election |
| `7_02_Ambalapuzha.Rmd` | The legend of Ambala**p**uzha | The legend of Ambala**pp**uzha |

## Notes / open items

- The six new chapters are **drafts** derived from the main-book content;
  review against how each activity is actually run in class, and add any
  local logistics (UCloud, file locations, timings).
- The main-book source filenames differ from the instructor filenames
  (e.g. main `2_12_MPMIntroAndSimulation.Rmd` ↔ instructor
  `2_10_MPMProjectionSimulation.Rmd`); the mapping above is by chapter
  title/content, not filename.
- Main-book Part 6 (Solutions/answers, ch 25–26) is deliberately not
  mirrored: the instructor book itself carries model answers inline.
