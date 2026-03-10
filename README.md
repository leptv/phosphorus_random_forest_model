## Overview

This repository contains a **Jupyter Notebook** implementing a Random Forest regression model accompanying the manuscript titled "...."  
The notebook analyzes **hydrological and geochemical monitoring data** from porewater collected at two sites (North and West) along the Wisconsin Riverbank on Blackhawk Island.  

The workflow includes correlation analysis, Random Forest modeling, and feature interpretability analyses.

---

## Data Input

- Input file: `full_groundwater_dataset.csv`  
- Contents: Environmental monitoring data, including hydrological and geochemical measurements from the two sites.  

---

## Analysis Workflow

1. **Correlation Analysis**  
   - Computes pairwise correlations among all environmental features.  
   - Generates **Figure S3** in the manuscript.  

2. **Random Forest Modeling**  
   - Trains a **Random Forest Regressor** using 5-fold cross-validation.  
   - Computes R², RMSE, and out-of-fold (OOF) predictions for evaluation.  
   - Generates **site-specific performance plots** (**Figure S1**).  

3. **Feature Interpretation**  
   - **Feature importance** comparison (Gini and permutation importance) → **Figure 3A**  
   - **SHAP values** for global interpretability → **Figure 3B**  
   - **Partial dependence plots** (PDPs) for each feature → **Figures 4 and S2**  

---

## Usage

1. Ensure the `full_groundwater_dataset.csv` file downloaded from the repository is in the same folder as the `random_forest_model.ipynb` Python script.  
2. Open the `random_forest_model.ipynb` Jupyter Notebook file and run all cells sequentially.  
3. Outputs generated:  
   - Correlation matrix and plots (Figure S3)  
   - Model performance metrics and site-specific plots (Figure S2)  
   - Feature importance comparison (Figure 3A)  
   - SHAP summary plots (Figure 3B)  
   - Partial dependence plots for each feature (Figure 4)  

---

## Requirements

- **Python 3.8+**  
- Python packages:  
  ```bash
  pip install pandas numpy scikit-learn shap matplotlib seaborn scipy
