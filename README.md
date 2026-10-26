# A Hybrid Data-Driven Approach for Analyzing and Predicting Inpatient Length of Stay

Code for the B.Sc. thesis and the preprint:

> **T. N. Chowdhury**, S. A. Mou, K. N. Rahman, "A Hybrid Data-Driven Approach for Analyzing and Predicting Inpatient Length of Stay in Health Care Centers," arXiv, 2025. [arXiv:2501.18535](https://arxiv.org/abs/2501.18535)

Hospitals can't plan beds and staff without knowing how long each patient will stay. This project predicts **length of stay (LOS) at admission** from 2.3 million de-identified New York inpatient records (SPARCS). It combines machine learning with process mining and simulation.

## Method

1. **Data:** demographics, diagnoses, treatments, costs and charges from SPARCS inpatient discharges.
2. **Big-data processing:** the data is cleaned and engineered with Apache Spark on AWS clusters.
3. **Dimensionality reduction:** PCA finds the factors that drive LOS most.
4. **Models:** Decision Tree, Logistic/Linear Regression, Random Forest, AdaBoost and LightGBM, compared with cross-validation.
5. **Patient flow:** the ML results feed process-mining and simulation analysis, which leads to resource-optimisation recommendations.

## Files

| File | Contents |
|---|---|
| `Patient2` | Main notebook: preprocessing, PCA, and the Decision Tree, Random Forest and AdaBoost models |
| `patient` | Earlier notebook: regression and decision-tree experiments |
| `try more` | Exploratory analysis and statistics (Plotly, SciPy, statsmodels) |
| `Untitled0.ipynb`, `Untitled1.ipynb` | Scratch notebooks |

These files are Jupyter notebooks written in Google Colab. Open them in Colab or Jupyter. Rename them with a `.ipynb` extension if needed.

## Data

The SPARCS data is public from the [New York State Department of Health](https://health.data.ny.gov/). It is not included here because of its size.

## Contact

Tasfia Noor Chowdhury · [tasfiaa.chowdhury@gmail.com](mailto:tasfiaa.chowdhury@gmail.com) · [ORCID](https://orcid.org/0009-0005-2074-1118)
