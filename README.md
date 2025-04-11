# Exploring Partial Domination in Graph Theory

This project explores the concept of **partial domination in graphs**, focusing on calculating and analyzing the smallest minimal dominating sets for specific graph families: **trees**, **paths**, and **cycles**.

The work combines combinatorics and data analysis, with the goal of finding patterns, conjectures, and possibly theoretical results from graph structures and their domination behavior.

---

## Project Structure

| File/Notebook | Description |
|---------------|-------------|
| `Trees_PartialDomination.ipynb` | Core notebook for generating all non-isomorphic trees up to a specified size and computing partial domination metrics. |
| `Trees_PartialDomination_Visualizations.ipynb` | Notebook for visualizing trees and their dominating sets using SageMath, and saving images organized by domination size and uniqueness. |
| `Paths_PartialDomination.ipynb` | Computes partial domination data for path graphs. |
| `Cycles_PartialDomination.ipynb` | Computes partial domination data for cycle graphs. |
| `PartialDomination_Permutations.ipynb` | Experimental notebook for checking permutations of sets for minimal p-domination across graphs. Kept for hsitory but ,ay be used for proof exploration or checking examples? |
| `df.csv` | Raw Pandas DataFrame export (CSV format) of computed domination values and data for each tree. Used for quick inspection and ease to pull uinto other analysis Jupyter Notebooks. |
| `partial_domination_results_14_vertices.xlsx` | Excel output with full data for all trees of size 14, including min/max domination set size, number of leaves, degree info, and whether the domination set is unique. |
| `trees_list.pkl` | Pickled list of SageMath tree objects (Graph instances), used for rebuilding trees in other notebooks. |
| `trees_edges_list.pkl` | Pickled list of edge lists (as Python tuples) corresponding to each tree. Used for rebuilding trees without full Sage Graph objects in otehr notebooks. |
| `README.md` | You're reading it! Describes the structure and purpose of the project. |

---

## What This Project Does

Each graph is analyzed to extract:
- **\( \gamma_p(G) \)** —> the size of the **smallest** \( p \)-dominating set
- \( \Gamma_p(G) \) —> the size of the largest minimal \( p \)-dominating set
- Difference between \( \gamma_p(G) \) and \( \Gamma_p(G) \)
- Structural properties (e.g. max degree, number of leaves)
- Whether the dominating set configuration is unique for that size + \( p \) value

Graph visualizations are exported and labeled by Excel row for easy reference in research and presentations.

---

## Research Goals

- Identify structural patterns that influence domination
- Compare tree types (star, path, cycle, balanced, etc.)
- Derive or verify known formulas for \( \gamma_p(G) \) in paths and cycles
- Propose and prove new formulas/conjectures
- Explore connections between graph structure and uniqueness of domination behavior

---

## How to Use Repo

1. Clone the repository:
   ```bash
   git clone https://github.com/nleali2022/trees-partial-domination.git

