# Bravais Lattice Prediction from XRD pattern
A project to identify Bravais crystal structures from the XRD patterns.  

## Problem statement and Datasets
The project was completed as an assignment for the [Nano281](https://github.com/materialsvirtuallab/nano281/tree/master/labs/lab3) course at UCSD. Datasets can be downloaded using Kaggle API (kaggle competitions download -c nano281fa2020).

## Feature selection
sin^2(2theta) is related to h^2+k^2+l^2 of the crystal planes and is used as features. Also since sin(theta) contains the phase information, coefficients from Discrete Sine Transform (DST) was used as features too.

## Used models and accuracy
Four classifier models (Naive Bayes, KNN, Random Forest Classfier and lightgbm (Gradient boost classifier)) were used to predict the lattice structure. The highest accuracy, ~60%, was obtained using the lighgbm classifier.
