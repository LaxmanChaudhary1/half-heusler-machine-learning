# Machine Learning for Half-Heusler Compounds

Research code, trained models, and post-processing notebooks for machine-learning studies of half-Heusler materials.

This repository is associated with the published work:

> **ML prediction of specific heat capacity for half-Heusler compounds**  
> *AIP Advances* **15**, 015306 (2025)

## Repository contents

- `code/` — training, evaluation, and post-processing notebooks/scripts, together with retained serialized model artifacts.
- `data/` — datasets used by the machine-learning workflows.
- `PostProcCv - Jupyter Notebook_files/` — legacy support files from an exported notebook view; retained for historical reproducibility.
- `.github/` — repository automation/workflow configuration.

The code directory contains workflows and saved estimators for quantities including lattice-related targets (`Alat`) and specific heat (`Cv`). Model files present in the repository include AdaBoost, decision-tree, Extra Trees, and Gaussian-process variants, together with post-processing notebooks.

## Research purpose

The project explores supervised machine-learning approaches for predicting materials properties of half-Heusler compounds from tabulated/material descriptors. The repository is best treated as a **research archive and reproducibility resource**, rather than as a packaged Python library.

## Suggested workflow

1. Inspect the datasets in `data/` and the preprocessing performed in the notebooks/scripts.
2. Use the notebooks in `code/` to reproduce model evaluation and post-processing.
3. Treat the committed `.pkl` files as historical trained-model artifacts tied to the software/data state used when they were generated.

## Reproducibility notes

- Serialized Python/scikit-learn model files can be version-sensitive. For rigorous reproduction, use compatible package versions and validate predictions against the original reported results.
- Jupyter checkpoint folders and Python cache files are generated artifacts and are excluded from future commits by `.gitignore`.
- This repository contains legacy research files; filenames and directory organization reflect the original working workflow.

## Citation

If this repository contributes to published work, please cite the associated paper:

**L. Chaudhary et al.**, “ML prediction of specific heat capacity for half-Heusler compounds,” *AIP Advances* **15**, 015306 (2025).

## Author

**Laxman Chaudhary**  
Computational materials physics and machine learning for materials.
