Mock Data Analysis — Linear & Quadratic - OLS, MLE, MCMC

Overview
- Two models: Linear y = a + b x and Quadratic y = a + b x + c x^2.
- Methods used:
  * Linear OLS: closed-form fit, residual variance, parameter errors.
  * Likelihood/χ^2 grid on (a, b): compute Δχ^2 = χ^2 − χ^2_min and draw credible regions at 2.30, 6.17, 11.8 (≈68.3%, 95.4%, 99.73% for 2 params).
  * Metropolis MCMC: posterior sampling for parameters, corner plots, credible sets derived from samples.
  * Model evidence: marginal likelihoods via log-sum-exp; compare models with Bayes factors (reported in log-space).
- Data files are NOT included. Results are preserved via the executed notebook outputs and saved figures.

Repo layout
- Linear_and_Quadratic_Model.ipynb   (executed with outputs)
- requirements.txt
- README.md

Requirements
- Python 3.x
- numpy
- matplotlib
- scipy
- corner

Install
    pip install -r requirements.txt


Run locally (with your own data)
1) Place the required data files in a local 'data/' folder (not included here). Update file paths in the notebook if needed.
2) Install packages:
       pip install -r requirements.txt
3) Launch Jupyter and run the notebook:
       jupyter lab
   (or 'jupyter notebook')

