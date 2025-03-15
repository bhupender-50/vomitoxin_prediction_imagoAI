# vomitoxin_prediction_imagoAI

## Preprocessing Steps
1. **Data Loading**: The dataset was loaded and inspected for missing values and inconsistencies.
2. **Handling Missing Values**: Missing values were imputed using the mean strategy.
3. **Normalization**: The spectral data was normalized using `StandardScaler`.

## Dimensionality Reduction
- **Feature Selection**: The top 20 features were selected using `SelectKBest` with `f_regression` as the scoring function.

## Model Selection, Training, and Evaluation
- **Model**: A Random Forest Regressor was chosen as the baseline model.
- **Training**: The model was trained using 5-fold cross-validation.
- **Evaluation**: The model achieved an MAE of 2350.57 

## Key Findings
- The model's performance is poor, as indicated by the high MAE and negative R² score.
- Possible reasons include insufficient data, noisy features, or inadequate model architecture.

## Suggestions for Improvement
1. Perform advanced feature engineering (e.g., spectral indices).
2. Experiment with more complex models (e.g., XGBoost, Neural Networks).
3. Use hyperparameter tuning to optimize model performance.
