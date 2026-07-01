# Liver Phantom Forward Modeling

## Overview

This project developed a machine learning and statistical modeling pipeline to predict the viscoelastic properties of liver-mimicking phantoms from material formulation variables and testing frequency.

The phantoms were fabricated using combinations of κ-carrageenan, agarose, and glycerol. Dynamic mechanical analysis (DMA) measurements were used to model storage modulus (G′), loss modulus (G″), and complex modulus across testing frequencies. The workflow supports the development of tunable tissue-mimicking phantoms for Magnetic Resonance Elastography (MRE) calibration and validation.

## Motivation

Reliable liver-mimicking phantoms are important for validating MRE-based stiffness measurements. Because phantom stiffness depends on multiple formulation variables, this project used regression and machine learning methods to better understand formulation–property relationships and guide future phantom design.

## Workflow

1. Loaded and cleaned DMA experimental data
2. Removed formulation groups outside the final experimental design
3. Reshaped repeated frequency measurements into long format
4. Created phantom-level train/test splits to reduce data leakage
5. Performed outlier detection and handling
6. Computed damping ratio for viscoelastic interpretation
7. Trained baseline and polynomial regression models
8. Compared global, categorical-frequency, and per-frequency modeling strategies
9. Evaluated model performance on held-out test data
10. Generated residual hotspot plots and adaptive sampling suggestions for future phantom fabrication

## Methods

- Data preprocessing and cleaning
- Long-format reshaping of frequency-based measurements
- Grouped train/test splitting by phantom formulation
- Outlier detection using univariable and multivariate approaches
- Feature engineering with polynomial and interaction terms
- Ordinary Least Squares regression
- Log-transformed target modeling
- Random Forest benchmarking
- Residual analysis
- Adaptive sampling for future experimental design

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Statsmodels
- SciPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Skills Demonstrated

- Machine learning pipeline development
- Data cleaning and feature engineering
- Regression modeling
- Statistical model interpretation
- Leakage-aware train/test splitting
- Scientific computing
- Biomedical data analysis
- Experimental design support

## Repository Status

This repository provides a high-level overview of the project.

The source code and dataset are not publicly available because this work was developed as part of ongoing NIH research.
