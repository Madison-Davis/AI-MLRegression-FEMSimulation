# Personal-MachineLearning-Regression-FEMSimulation

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
