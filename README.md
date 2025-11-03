# Predicting Beats Per Minute (BPM)

<div style="display: flex; width: 100%;">
    <img width="1370" height="172" alt="image" src="https://github.com/user-attachments/assets/8ff9d144-22f9-4bce-8586-be1c37bc0b8d" />
</div>

This repository contains a solution for the Kaggle competition [Playground Series – S5E9](https://www.kaggle.com/competitions/playground-series-s5e9), where the task is to predict the **BeatsPerMinute** (BPM) for audio tracks using tabular audio features.

## Overview

- **Task**: Regression — predict BPM for audio tracks.  
- **Input**: Tabular features describing audio tracks.  
- **Datasets**:
  - **Train**: ~500k samples with `BeatsPerMinute`.  
  - **Test**: ~100k samples without target.  
- **Evaluation Metric**: RMSE.

## Models compared
- Fully connected neural network (Keras) — 64 → 32 → 1.  
- Linear Regression (scikit-learn).  
- CatBoostRegressor (gradient boosting).  

## Results

Linear Regression produced the best validation RMSE among the tested models and was used to generate the final submission, which is approximately equal to the best scores of other contestants.
