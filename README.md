# Outcome Prediction Experiments

This repository contains the results of outcome prediction experiments comparing different feature sets derived from prior literature and from the closest related work.

The experiments were conducted using *League of Legends* match data obtained from the Oracle’s Elixir repository, covering the 2023 and 2024 competitive seasons.

## Regions

The analysis includes data from the following major regions:

* LCK
* LCS
* LEC

## Experimental Setup

Outcome prediction models were trained using matches from 2023 and evaluated on matches from 2024, ensuring a temporal split between training and testing data.

## Files

### `GSCV_train23_Test24.csv`

This file presents the accuracy results obtained through a GridSearchCV procedure applied to the following models:

* Decision Tree
* Random Forest
* Multi-Layer Perceptron (MLP)
* LightGBM

The training set consists of matches from 2023, while the test set consists of matches from 2024.

### `RF_LiteratureBased_FeatureSet.csv`

Contains the accuracy results obtained using a feature set derived from prior literature, including role-based performance representations and task-oriented feature design.

### `RF_RelatedWork_FeatureSet.csv`

Contains the accuracy results obtained using a feature set based on the methodology proposed in the closest related work.

## Notes

* All feature sets were implemented to ensure a fair comparison under the same experimental conditions.
* The naming of feature sets is intentionally generic to preserve anonymity during the review process.
