k-Nearest Neighbours — Effect of Distance Weighting on Decision Boundaries
Overview

This repository contains the code and experimental materials for a university-level Machine Learning coursework assignment examining how different voting schemes influence the behaviour of the k-Nearest Neighbours (kNN) classifier. The study focuses on the contrast between uniform voting and distance-weighted voting and analyses their impact on decision boundary geometry, error structure, and generalisation performance.

Project Objective

The objective of this project is to isolate and analyse the effect of the neighbour voting strategy in kNN classification. Rather than comparing multiple algorithms or tuning the number of neighbours, the work fixes 
𝑘
k and varies only the voting scheme. This design enables a precise examination of how local weighting alters inductive bias, variance, and decision geometry.

The study addresses the following questions:

How does distance weighting affect the smoothness and stability of decision boundaries?

When does increased local sensitivity improve or degrade performance?

How do error patterns differ between voting schemes in overlapping regions?

Repository Structure

notebooks/
Jupyter notebook containing all experiments, visualisations, and evaluations.

figures/
Plots generated during the experiments and used in the final report.

report/
Final written tutorial submission (PDF or web-based format).

Dataset

A synthetic two-dimensional dataset is used to allow direct visualisation of neighbourhood structure and decision boundaries. The data includes controlled class overlap and label noise to highlight differences in robustness between voting schemes. Data generation is fully reproducible within the provided notebook.

Methodology

Two kNN models are evaluated using the same distance metric and neighbourhood size. The only difference between models is the voting mechanism: uniform voting versus distance-weighted voting. Performance is assessed using accuracy and macro-averaged F1 score. Additionally, decision boundary plots and error visualisations are used to analyse geometric and failure-mode behaviour.

Reproducibility

All results are fully reproducible. Running the provided notebook end-to-end will regenerate all figures and quantitative outputs reported in the tutorial. Random seeds are fixed, and no manual preprocessing steps are required.

Requirements

The experiments require a standard Python scientific computing environment, including NumPy, Matplotlib, and scikit-learn. No specialised hardware or proprietary software is necessary.

Usage

Run the notebook in the notebooks/ directory from top to bottom.

Inspect the generated figures to analyse decision boundary behaviour.

Refer to the report in the report/ directory for interpretation and theoretical discussion.

License

This project is provided for educational and academic use. See the LICENSE file for detailed terms of use.
