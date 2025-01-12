# Regression
# Part 1: Linear Regression on Boston Housing Data
See code for implementation.  More details shown below:</br>
Caveat: understand linear modeling is usually not the most accurate in a binary-output model, where a probit or logit may do better.  In this instance, we value based on a linear scale, so this does not apply.
77% Accuracy using Linear Regression

Dataset: https://www.kaggle.com/datasets/fedesoriano/the-boston-houseprice-data

Input features in order:

CRIM: per capita crime rate by town
ZN: proportion of residential land zoned for lots over 25,000 sq.ft.
INDUS: proportion of non-retail business acres per town
CHAS: Charles River dummy variable (1 if tract bounds river; 0 otherwise)
NOX: nitric oxides concentration (parts per 10 million) [parts/10M]
RM: average number of rooms per dwelling
AGE: proportion of owner-occupied units built prior to 1940
DIS: weighted distances to five Boston employment centres
RAD: index of accessibility to radial highways
TAX: full-value property-tax rate per 
10
,
000
[
/10k]
PTRATIO: pupil-teacher ratio by town
B: The result of the equation B=1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town
LSTAT: % lower status of the population
Output variable:

MEDV: Median value of owner-occupied homes in 1000's

# Part 2: Ridge Regression on Steel Industry Data
See code for implementation.  More details shown below:</br>
97% Accuracy using Ridge Regression Purpose: be able to predict energy consumption of steel factory based on specified criteria, ultimately hoping to make consumption more efficient
# Part 3: RANSAC Regression on FEM Simulated Data
See code for implementation.  More details shown below:</br>
100% Accuracy using RANSAC (Random Sample Consensus) Regressor
Goal: predict the outputs of a finite element model simulation based on stress results.  Four outputs were tested individually, and all four had the same accuracies: MTT, MRT, MTC, MRC

Dataset: https://www.kaggle.com/datasets/daalgi/fem-simulations?datasetId=2744

Context
Engineers use numerical models to analyze the behavior of the systems they are studying. By means of numerical models you can prove whether a design is safe or not, instead of making a prototype and testing it. This gives you great flexibility to modify parameters and to find a cheaper design that satisfies all the safety requirements.

But when the models are too complex, the numerical simulations can easily last from a few hours to a few days. In addition, during the optimization process you might need a few tens of trials. So in order to simplify the process we can build a simple 'surrogate' model that yields similar results to the original one. Here's when Machine Learning comes in!

Content
The dataset contains the data of about 6000 numerical simulations (finite element models, FEM). It must be pointed out that there is no noise in the data, that is, if we run again the simulations we'd get the same results. There are 9 input parameters and 4 output results.

Inputs (continuous and positive values):
(1) load parameters: ecc, N, gammaG.
(2) material parameters: Esoil, Econc.
(3) geometry parameters: Dbot, H1, H2, H3.

Outputs (continuous values):
(1) stress related results: Mrt, Mtt, Mrc, Mtc.
