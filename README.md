Project Title

Double Machine Learning for Causal Inference Using Python

Project Description

This project implements Double Machine Learning methodology for causal inference using Python.
The objective of the project is to estimate both the Average Treatment Effect and the Conditional Average Treatment Effect in a high dimensional setting using machine learning based nuisance models.
The project follows the Double Machine Learning framework with cross fitting to reduce bias from regularization.

Dataset Description

Synthetic data is generated with a sample size of 10000 observations.
The dataset includes a binary treatment variable, a continuous outcome variable, and multiple covariates.
The data generating process explicitly includes heterogeneous treatment effects to enable Conditional Average Treatment Effect evaluation.

Methodology

The project uses Double Machine Learning with cross fitting.
Separate machine learning models are used to estimate the outcome regression and treatment assignment models.
K fold cross fitting is applied to obtain residuals that are used in the final stage estimation.
The final stage regression estimates the causal parameters using orthogonalized moments.

Estimands

Average Treatment Effect
Conditional Average Treatment Effect

Baseline Methods

Naive Ordinary Least Squares
Propensity Score Matching
Inverse Probability Weighting

Simulation Study

A Monte Carlo simulation study with 100 independent runs is conducted.
In each run, data is generated, causal effects are estimated using all methods, and results are stored.
The simulation compares bias, variance, and coverage probability across methods.

Evaluation

Estimated effects are compared with true data generating parameters.
Bias is computed as the difference between estimated and true effects.
Variance and empirical coverage are calculated across simulation runs.

Files in the Repository

DML_Devisree.ipynb contains the full implementation
The notebook includes data generation, model estimation, simulation loops, and result summaries

Requirements

Python version 3 or above
Jupyter Notebook
NumPy
Pandas
Scikit learn
Matplotlib

How to Run

Install Python and required libraries
Open DML_Devisree.ipynb in Jupyter Notebook
Run all cells to reproduce the simulation study and results

Deliverables

Complete Double Machine Learning implementation
Monte Carlo simulation results
Text based explanation of methodology and analysis

Project Scope

This project is intended for academic and learning purposes.
The implementation focuses on demonstrating the principles of Double Machine Learning and causal inference.

Author

Devisree G

License

This project is free to use for educational purposes only
