# NeurIPS - Ariel Data Challenge 2025

## Description
This repository focuses on learning and experimentation for the **Ariel Data Challenge 2025** at NeurIPS. The main objective is to predict exoplanet transmission spectra using time-series data from the AIRS-CH0 and FGS1 instruments, along with related stellar and planetary metadata. The notebooks cover the full pipeline from data exploration and feature extraction to baseline models, deep learning, and ensembling.

## Competition Link
Learn more on Kaggle: **https://www.kaggle.com/competitions/ariel-data-challenge-2025**.

## Learning Goals
- Understand the competition data structure and file formats (CSV, Parquet, metadata).
- Build a solid baseline for transmission spectrum prediction.
- Apply feature engineering to instrument time-series data.
- Explore stronger models (deep learning, ensembling).

## Notebook Structure
1. **Setup & Environment**: Install and import required libraries.
2. **Load & Verify Data**: Load core data (CSV & Parquet), ADC calibration, and schema checks.
3. **Exploratory Data Analysis (EDA)**: Visualize transmission spectra, stellar parameters, and time-series.
4. **Preprocessing & Feature Engineering**: Extract time-series features from calibrated signals, detrending, and descriptive stats.
5. **Baseline Model**: Ridge Regression, XGBoost, and LightGBM with PCA spectrum features.
6. **Deep Learning Model**: InceptionTime implementation for time-series spectrum prediction.
7. **Evaluation & Hyperparameter Tuning**: Cross-validation and tuning (scikit-learn & Keras Tuner).
8. **Ensembling & Submission**: Combine models and generate a competition submission file.

## How to Run
1. **Prepare Data**: Ensure the dataset folder structure matches the notebook paths (e.g., `/kaggle/input/ariel-data-challenge-2025/`).
2. **Install Libraries**: Run install cells outside Kaggle (`pip install kaggle pyarrow lightgbm xgboost keras-tuner`).
3. **Run the Notebook**: Execute cells in order from top to bottom.
4. **Training & Evaluation**: The notebook includes baselines, deep learning, and hyperparameter tuning.
5. **Submission**: Save predictions to `submission.csv` in the competition format.

## Suggested Learning Flow
1. **Read rules & evaluation** on the Kaggle competition page.
2. **Run EDA** to understand spectral patterns and time-series data.
3. **Start with a baseline** before adding model complexity.
4. **Iterate & document** experiments for reproducibility.

## Library Requirements
- numpy
- pandas
- pyarrow
- matplotlib
- seaborn
- scikit-learn
- xgboost
- lightgbm
- tensorflow
- torch (optional)
- keras-tuner

## Important Notes
- Ensure data paths are correct, especially when running outside Kaggle.
- The notebook can be extended with additional features, models, or ensembling techniques.
- For test inference, make sure calibration and feature extraction align with the test data format.

## References
- [Ariel Data Challenge 2025 - Kaggle](https://www.kaggle.com/competitions/ariel-data-challenge-2025)
- [Ariel Mission](https://arielmission.space/) 
