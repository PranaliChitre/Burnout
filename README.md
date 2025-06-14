# Burnout
This repository contains an advanced machine learning solution for predicting MotoGP lap times using a sophisticated ensemble of models and domain-specific feature engineering. The solution leverages XGBoost, LightGBM, CatBoost, and a Neural Network in a weighted ensemble to maximize predictive accuracy.

🚀 Key Features
Advanced Data Preprocessing

Intelligent handling of missing values (forward-fill + median for lap times, mode for categoricals)

Robust encoding of categorical variables (teams, bikes, weather conditions)

Domain-Specific Feature Engineering

Track Characteristics: Corner density, speed per corner, track flow

Tire Strategy: Grip & durability multipliers, tire mismatch penalty

Weather Modeling: Impact of rain, temperature effects

Rider Performance Metrics: Win rate, podium rate, career momentum

Session Dynamics: Qualifying vs. race multipliers

Grid Position Psychology: Front-row advantage, back-of-grid pressure

Sophisticated Feature Selection

Variance Thresholding (removes low-variance features)

Statistical Selection (F-test regression)

Cross-validated importance ranking

Ultra-Ensemble Model

XGBoost (35% weight) – Best for structured data

LightGBM (30% weight) – Fast & efficient

CatBoost (25% weight) – Handles categoricals natively

Neural Network (10% weight) – Captures complex interactions

Advanced Post-Processing

Weather-based adjustments (rain → slower times)

Session-specific corrections (qualifying vs. race)

Outlier clipping (percentile-based)

Notebook link : https://www.kaggle.com/code/pranalichitre/notebook911854fcba?scriptVersionId=245457168
