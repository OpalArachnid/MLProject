# Predicting Tsunami Occurrences from Earthquake Data

## Overview
This project predicts the likelihood of a tsunami following an earthquake using machine learning. Data from 1,000 earthquakes (1995-2023) includes features such as magnitude, MMI (Modified Mercalli Intensity) index, depth, and geographic coordinates.

## Dataset
The dataset, sourced from Kaggle and the USGS Earthquake Catalog, includes:
- **Magnitude**: Earthquake strength.
- **MMI Index**: Shaking intensity at specific locations.
- **Depth**: Depth of the earthquake in kilometers.
- **Latitude & Longitude**: Geographic location.

The target variable is binary: `1` for a tsunami warning, `0` otherwise.

## Methods
- **Models**: Logistic Regression and Random Forest.
- **Metrics**: Accuracy, Precision, Recall, and Confusion Matrix.
- **Cross-Validation**: k-fold and Repeated k-fold to validate performance and reduce bias.
- **Preprocessing**: Feature selection and handling missing/irrelevant data.

## Results
- Logistic Regression accuracy: **0.69-0.73**; Random Forest accuracy: **0.64-0.7**.
- Final recall (Random Forest): **0.6**, prioritizing reduced false negatives to improve safety.
- Random Forest was more robust after parameter fine-tuning.

## Conclusion
Despite dataset challenges (imbalanced labels, limited size), the random forest model provided better recall and robustness. Future improvements include adding features, addressing imbalance, and exploring advanced models.
