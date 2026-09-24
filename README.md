# SPE DSEATS Africa Datathon 2026

## Overview

This repository contains our submission for the SPE DSEATS Africa Datathon 2026. The challenge centered on oil presence classification, and our team built a multi-model machine learning pipeline enhanced with physics-informed corrections to improve prediction accuracy over a purely data-driven baseline.

## Team

- Iwuoha David
- Mercy Owen
- Moyosore Olawoye

## Approach

Our pipeline combined several gradient-boosting architectures into a stacked ensemble:

- **LightGBM**
- **XGBoost**
- **CatBoost**
- **Stacking ensemble** combining the above base learners

On top of the standard ML pipeline, we applied physics-informed corrections grounded in domain knowledge of oilfield behavior, rather than relying on the models to learn these relationships purely from data.

## Results

The domain-corrected Part 2 submission achieved a **+6.9% F1 improvement** over the uncorrected baseline, demonstrating the value of embedding physical reasoning into a data-driven pipeline.

## Repository Structure

```
.
├── data/               # Raw and processed datasets
├── notebooks/          # Exploratory analysis and model development
├── src/                # Pipeline and model code
├── models/             # Trained model artifacts
└── README.md
```



## Tech Stack

- Python
- LightGBM, XGBoost, CatBoost
- Physics-informed feature engineering / correction layer

## Acknowledgements

Built for the SPE DSEATS Africa Datathon 2026.
