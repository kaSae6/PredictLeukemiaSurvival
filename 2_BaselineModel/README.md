# Baseline Model

**[Notebook](baseline_model.ipynb)**


## Model Choice

Linear Regression was chosen as the primary baseline because:
    Simplicity: Easiest to understand and interpret - coefficients show direct relationship between clinical features and survival time
    Fast and efficient: Quick to train and make predictions
    Medical relevance: Linear relationships between biomarkers and outcomes are common in clinical data

Random Forest was added as a secondary baseline because:
    Captures non-linear relationships: Can model complex interactions between features without manual feature engineering
    Robust to outliers: Medical data often contains extreme values; RF handles these naturally
    Feature importance: Provides rankings of which clinical variables matter most  



## Feature Selection

The overall survival prediction will be based on the generation of a risk score through the evaluation of the status (alive or dead) OS_STATUS, as event indicator and with the time measurements of survival in years OS_YEARS after last follow-up as time variable.

Feature selection could be done randomly, or by differentiation of weighting risk-factors which would be highly desired in health-related fields.

Some main features of AML described in literature are the presence of blast cells in percentage (column 'BM_BLAST'), low concentration of Hemoglobine levels, resulting in anemia (column 'HB') as well as low levels of platelets (column 'PLT').

## Evaluation

We will evaluate both baseline models using standard regression metrics:
Mean Absolute Error (MAE): Average absolute difference between predicted and actual survival times
* Lower is better, measured in years
* Easy to interpret: "model is off by X years on average"

Root Mean Squared Error (RMSE): Penalizes larger errors more heavily
* Lower is better, measured in years
* More sensitive to outliers than MAE

R² Score: Proportion of variance explained by the model
* Range: -∞ to 1.0 (1.0 is perfect)
* Negative values mean model performs worse than just predicting the mean

Note: These models only predict survival time for patients who experienced the event. This is a limitation but provides a simple baseline for comparison.

## BASELINE MODEL SUMMARY & BENCHMARKS


Best performing baseline model: Random Forest
Benchmark to beat:
  - Mean Absolute Error: 1.284 years
  - Root Mean Squared Error: 1.739 years

Key insights from baseline analysis:
  • Random Forest outperforms Linear Regression (MAE: 1.284 vs 1.295)
  • Non-linear relationships exist in the data
  • Most important features: ('PLT', np.float64(0.465)), ('HB', np.float64(0.383)), ('BM_BLAST', np.float64(0.151))

The advanced survival model should beat the MAE = 1.284 years
