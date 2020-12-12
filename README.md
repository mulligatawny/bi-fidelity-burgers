# Bi-fidelity Approximation: Burgers' Equation

The bi-fidelity approximation applied to the 1D inviscid Burgers' equation. The input uncertainty is in the variance of the Gaussian initial condition.

The code demonstrates the use of a linear transformation that uses domain-specific knowledge (i.e. the shock locations), which is shown to introduce additional errors that are mitigated using a two-stage approach (`bi_fidelity_two_stage.ipynb`).

The interpolative decomposition used is from Martinsson et al. (https://www.pnas.org/content/104/51/20167), and the package documentation is found here: https://docs.scipy.org/doc/scipy/reference/linalg.interpolative.html. For a CFD application of the bi-fidelity approximation, see Fairbanks et al.: https://arxiv.org/abs/1808.05742.

File manifest:

`data` contains LF and HF matrices saved for outer loop activities.

`figures` contains images produced from the Burgers' code.

`bi_fidelity_burgers.ipynb` is the main notebook.

`bi_fidelity_two_stage.ipynb` contains the two-stage approach.

`brief_summary.pdf` is a short report summarizing the problem.

