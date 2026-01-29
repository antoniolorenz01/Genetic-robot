# Notebook Guide (English)

The main artifact in this repository is a Jupyter notebook that demonstrates **Genetic Programming (GP)** for synthesizing a small, interpretable controller for a robot moving in a **grid-world**.

## What the Notebook Does
- Defines a simulated 2D grid environment with a **start** position and a **target**.
- Represents a controller as a **symbolic expression tree** (Genetic Programming individual).
- Evolves controllers with a **multi-objective** evolutionary algorithm (Pareto optimization), typically balancing:
  - **Distance to the goal** (lower is better).
  - **Controller complexity** (e.g., number of nodes in the GP tree; lower is better).
- Extends the environment to include **obstacles** and re-trains/evaluates in that setting.
- Produces plots/visuals such as a **Pareto frontier** and example trajectories.

## How to Use It
1. Install dependencies: `pip install -r requirements.txt`
2. Launch Jupyter: `jupyter lab`
3. Open the notebook in `notebooks/`.

## Expected Outputs
Depending on which sections you run, you should see:
- Evolution logs/statistics (fitness progression).
- A scatter plot of the Pareto frontier.
- A simulated trajectory of a selected “best” individual.
- Optional: a rendered tree representation of the symbolic controller (Graphviz).
