# Predicting Beats Per Minute (BPM)

<div style="display: flex; width: 100%;">
    <img width="1370" height="172" alt="image" src="https://github.com/user-attachments/assets/8ff9d144-22f9-4bce-8586-be1c37bc0b8d" />
</div>

This repository contains a solution for the Kaggle competition [Playground Series – S5E9](https://www.kaggle.com/competitions/playground-series-s5e9), where the task is to predict the **BeatsPerMinute** (BPM) for audio tracks using tabular audio features.

## Overview

The task is a **regression** problem: predict the beats per minute (BPM) of audio tracks. Inputs are tabular features that describe each track. The training dataset contains approximately 500k samples with the BeatsPerMinute target, and the test set contains about 100,000 samples without target values. Model performance is evaluated using root mean squared error (RMSE).

## Models compared
- Fully connected neural network (Keras) — 64 → 32 → 1.  
- Linear Regression (scikit-learn).  
- CatBoostRegressor (gradient boosting).  

## Results

Linear Regression produced the best validation RMSE among the tested models and was used to generate the final submission, which is approximately equal to the best scores of other contestants.
