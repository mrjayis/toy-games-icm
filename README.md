# Poker Toy Games & ICM

An interactive web app for understanding GTO toy games and how they inform tournament poker strategy through the lens of ICM.

**Live app:** https://mrjayis.github.io/toy-games-icm/

## What's inside

**Solving Toy Games** — The method. Where money lives (stacks vs the pot, split into each player's EV) and why you control your opponent's EV rather than your own. A "nemesis" graph built from the always-call and always-fold lines, a step-by-step pruning of the KK/33 vs 88 game tree, an indifference solver for that game, and a red/yellow/blue arrow calculator: point red at your opponent's risk, yellow at the pot before it, blue at the pot after it. Then yellow/blue is your winning frequency, red/blue your losing frequency, and yellow:red your value:bluff (or call:fold) ratio.

**Polarized vs Bluffcatcher** — The foundational river toy game. Adjust bet size and watch MDF, bluff frequency, and value EV update in real time with SVG charts.

**Trap Hands** — Extends the base model with traps in the defender's range. Visualizes how optimal bet sizing shrinks as trap frequency increases, with the formula `s* = 1/√(2T) − 1`.

**ICM & Nash Limitations** — Why Nash equilibrium guarantees break down in tournament poker. Includes an EV leakage calculator using a proper Malmuth-Harville ICM model (bitmask DP) and a risk premium visualizer showing how calling thresholds shift under tournament pressure.

**Tournament Play** — Ties it together: ICM-adjusted MDF, bluff frequency curves, and a 13×13 hand range grid showing which hands to call in cash games vs on the bubble.

## References

- [How to Solve Toy Games — GTOWizard](https://blog.gtowizard.com/how-to-solve-toy-games/)
- [The Limitations of Nash Equilibrium in ICM Spots — GTOWizard](https://blog.gtowizard.com/the-limitations-of-nash-equilibrium-in-icm-spots/)
