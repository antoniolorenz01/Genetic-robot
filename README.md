# Genetic Robot — Symbolic Controller Synthesis (Genetic Programming)

This repository contains a **Jupyter notebook** exploring **Genetic Programming (GP)** to *symbolically synthesize* an interpretable controller for a simple robot in a grid-world environment, optimized with **multiple objectives**.

The work uses **DEAP** (Genetic Programming + multi-objective evolutionary algorithms) and includes:
- A basic grid environment (start → target).
- A multi-objective fitness setup (e.g., **distance-to-goal** vs **controller complexity**).
- A variant with **obstacles**.
- Visualizations such as a **Pareto frontier** and (optionally) **controller trees** with Graphviz.

## Quick Start

### 1) Setup
Requirements: Python 3.9+.

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

If you want tree visualizations, install Graphviz on your system:
- Debian/Ubuntu: `sudo apt-get install graphviz`
- macOS (Homebrew): `brew install graphviz`

### 2) Run the Notebook
```bash
jupyter lab
```
Then open: `notebooks/symbolic_synthesis_multiobjective_robot_controller.ipynb`

## Repository Layout
- `notebooks/` — main notebook (the project lives here).
- `docs/` — short supporting docs (English guide/overview).

## Notes
- The notebook narrative is currently **in Spanish**. `docs/NOTEBOOK.md` provides an English guide to what’s inside.

## License
No license file is included yet. Before publishing publicly, pick a license (for example: MIT, Apache-2.0, GPL-3.0) and add a `LICENSE` file.
