# Credit Risk Analysis

## Overview

This project uses the credit card credit dataset from LendingClub to over-sample the data using the RandomOverSampler and SMOTE algorithms, and under-sample the data using the ClusterCentroids algorithm in the notebook `credit_risk_resampling.ipynb`.

Next the notebook uses a combination of over and under-sampling using the SMOTEEN algorithm on the same dataset.

The notebook, `credit_risk_ensemble.ipynb` takes the same dataset to compare two machine learning models to reduce bias using the BalancedRandomForestClassifier and EasyEnsembleClassifier objects from the imbalance-learn library to predict credit risk.

This report will evaluate the performance of these models followed by a recommendation on which models would be best for predicting credit risk.

## Results

The following list shows the results of the balanced accuracy scores and the precision and recall scores of all six machine learning models.

- Random Over Sampler

    <img src="./images/random_o_sampler_res.png" alt="Random Oversampler Results" width="500"/>

  - Balanced Accuracy Score: 0.65
  - Precision Score: 0.99
  - Recall Score: 0.67
  <p>

- SMOTE

    <img src="./images/smote_o_sampler_res.png" alt="SMOTE Results" width="500"/>

  - Balanced Accuracy Score: 0.61
  - Precision Score: 0.99
  - Recall Score: 0.66
  <p>

- Cluster Centroids

    <img src="./images/cluster_centroids_u_sampler_res.png" alt="Cluster Centroids Results" width="500"/>

  - Balanced Accuracy Score: 0.51
  - Precision Score: 0.99
  - Recall Score: 0.44
  <p>

- SMOTEENN

  <img src="./images/smoteenn_o_u_sampler_res.png" alt="SMOTEENN Results" width="500"/>

  - Balanced Accuracy Score: 0.64
  - Precision Score: 0.99
  - Recall Score: 0.58
  <p>

- Balanced Random Forest Classifier

    <img src="./images/balanced_random_classifier_res.png" alt="Balanced Random Classifier Results" width="500"/>

  - Balanced Accuracy Score: 0.79
  - Precision Score: 0.99
  - Recall Score: 0.91
  <p>

- Easy Ensemble Classifier

    <img src="./images/easy_ensemble_classifier_res.png" alt="Easy Ensemble Classifier Results" width="500"/>

  - Balanced Accuracy Score: 0.93
  - Precision Score: 0.99
  - Recall Score: 0.94
  <p>

## Summary

The following table shows the results for all 6 of our models. The classifier models easily outperformed the random sampling models with the Random Over Sampler slightly outperforming the SMOTEEN sampler.

Even though the Balanced Random Forest Classifier performed really well compared to the random samplers, the Easy Ensemble Classifier had the best results overall and is the recommended model for predicting credit risk.

<img src="./images/summary_table.png" alt="Summary Table" width="500"/>
