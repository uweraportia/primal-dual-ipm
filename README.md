# Primal-Dual Interior Point Methods for Linear Programming

**Author:** Amr Yasser  
**Affiliation:** Dept. of CSAI, Zewail City of Science and Technology, Egypt  

---

## Overview

This repository contains a detailed implementation, analysis, and case studies of **primal-dual interior point methods (IPMs)** for solving linear programming (LP) problems. 

Three primal-dual IPM variants are implemented from scratch in Python:

1. **Central Path IPM (Fixed Parameters)** – baseline method with constant step size and centering parameter.
2. **Central Path IPM (Adaptive Parameters)** – step size and centering parameter adapt based on residuals.
3. **Mehrotra Predictor–Corrector** – the practical state-of-the-art method with predictor-corrector updates.

The implementations are validated against the SciPy IPM solver, and the code produces reproducible results with detailed plots and pseudocode for each algorithm.

---

## Repository Structure

```text
primal-dual-ipm/
├── figures/               # All figures (PDF + PNG) for main report and appendix
├── notebook/              # Jupyter notebook with implementations and experiments
├── LICENSE                # Creative Commons BY-SA 4.0 license
├── main.tex               # LaTeX report
├── references.bib         # BibTeX references
├── README.md              # Project overview (this file)
└── .gitignore             # Git ignore rules
````

* `figures/` contains convergence plots, primal-dual trajectories, and appendix figures for each LP case study.
* `notebook/interior_point_methods.ipynb` contains all algorithm implementations and interactive experimentation.
* `main.tex` compiles the full report including introduction, algorithms, case studies, results, appendix pseudocode, and figures.
* `LICENSE` applies a **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)** license to this work.

---

## Case Studies

Three LPs are used to demonstrate the methods:

1. **Simple 2D LP** – a toy problem for visualizing the central path.
2. **Resource Allocation LP** – medium-scale LP mimicking practical allocation problems.
3. **Diet Problem** – classic LP benchmark from operations research.

Full-page figures for each LP are included in the appendix of the report.

---

## Features

* Complete implementations of three primal-dual IPMs.
* LU-based Revised Simplex Phase II and Phase I initialization pseudocode.
* Reproducible convergence plots and primal-dual trajectory visualizations.
* Adaptive and predictor-corrector variants for practical efficiency.
* Detailed LaTeX report ready for submission or publication.
* Clear, frame-based pseudocode in the appendix for readability.

---

## Running the Report

1. **Compile LaTeX**:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

2. **Run Jupyter Notebook**:

```bash
jupyter notebook notebook/interior_point_methods.ipynb
```

All figures in `figures/` are generated from the notebook.

---

## Full Report

You can view the full report here: [Primal-Dual Interior Point Methods (PDF)](https://amr-yasser226.github.io/primal-dual-ipm/final.pdf)

---

## License

This work is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) License](LICENSE).


---

## References

All references used in this report are included in `references.bib` and cited throughout the LaTeX document.
