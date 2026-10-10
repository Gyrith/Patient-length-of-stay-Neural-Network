# Patient Length of Stay Prediction

Neural network (Keras) that predicts hospital length of stay in days, comparing SGD, RMSprop and Adam optimizers.

## Files
- `nn_fundamentals_lab.ipynb`: lab notebook
- `patient_los.csv`: dataset (100,000 patients)

## Method
- 80/20 train/test split; numeric features scaled, categorical features one-hot encoded
- Model: Dense(64) → Dense(32) → Dense(1), MSE loss, 50 epochs
- Best model chosen by validation loss, then scored on the test set

## Results
| Metric | Value |
|---|---|
| Best optimizer | RMSprop |
| Test MAE | 1.68 days |
| Test RMSE | 2.38 days |
| Within 2 days | 72.4% |