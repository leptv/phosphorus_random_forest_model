# README

# Overview

# 

# This repository contains a Python script in Jupyter Notebook format that implements a Random Forest regression model accompanying the manuscript. The notebook is designed to analyze hydrological and geochemical monitoring data from porewater collected along the hyporheic zone at two sites (North and West) along the Wisconsin Riverbank on Blackhawk Island.

# 

# The notebook performs the following:

# 

# Data Input:

# 

# Takes the file full\_groundwater\_dataset.csv as input.

# 

# This file contains environmental monitoring data, including hydrological and geochemical measurements from the two sites from 2023-2025.

# 

# Data Analysis:

# 

# Conducts correlation analysis among all environmental features, generating Figure S3 in the manuscript.

# 

# Random Forest Modeling:

# 

# Trains a Random Forest Regressor using 5-fold cross-validation.

# 

# Evaluates model performance, computing R², RMSE, and out-of-fold predictions.

# 

# Generates site-specific performance plots (Figure S2).

# 

# Feature Interpretation:

# 

# Calculates and visualizes feature importance (Figure 3A).

# 

# Computes SHAP values for interpretability (Figure 3B).

# 

# Generates partial dependence plots for each feature (Figure 4).

# 

# Usage

# 

# Place the full\_groundwater\_dataset.csv file in the working directory.

# 

# Open the Jupyter Notebook and run each cell sequentially.

# 

# The notebook will automatically produce:

# 

# Correlation matrix and plots (Figure S3).

# 

# Model performance metrics and plots per site (Figure S2).

# 

# Feature importance comparison plot (Figure 3A).

# 

# SHAP summary plots (Figure 3B).

# 

# Partial dependence plots (Figure 4).

# 

# Requirements

# 

# Python 3.8+

# 

# Jupyter Notebook

# 

# Packages: pandas, numpy, scikit-learn, shap, matplotlib, seaborn, scipy

