# Credit Risk Analysis

## Overview

This project uses the credit card credit dataset from LendingClub to oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm in the notebook `credit_risk_resampling.ipynb`.

Next the notebook uses a combination of over and undersampling using the SMOTEEN algorithm on the same dataset.

The notebook, `credit_risk_ensemble.ipynb` takes the same dataset and to compare two machine learning models to reduce bias using the BalancedRandomForestClassifier and EasyEnsembleClassifier objects from the imbalance-learn library to predict credit risk.

This document will evaluate the performance of these models followed by a recommendation on whether they should be used to predict credit risk.

## Results

TODO: add screen shots and descibe results found.

## Summary

TODO: add recommendations

## Development Notes

Using the Balanced Random Forest Classifier in the ML env, was erroring out on shaping the X data even after installing the correct versions of scikit-learn.

To resolve this error, the Python 3 kernel was updated as follows:

`conda create -n data-b-17-supervisedlearning python=3.10 imbalanced-learn=0.9 ipykernel=6.15 jupyterlab=3.4 numpy=1.23 pandas=1.4 scikit-learn=1.1 -c conda-forge --strict-channel-priority`
