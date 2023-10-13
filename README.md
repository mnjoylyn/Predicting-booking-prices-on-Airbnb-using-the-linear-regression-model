# Predicting-booking-prices-on-Airbnb-using-the-linear-regression-model
Let’s say we want to build a model to predict booking prices on Airbnb. Between linear regression and random forest regression, which model would perform better and why?
import numpy as np
import pandas as pd

n_samples = 5  
n_features = 5

X_new = np.random.rand(n_samples, n_features)
print("New Data for Prediction (X_new):")
print(X_new)

y_pred_linear = linear_reg.predict(X_new)
data_dict = {f'Feature_{i}': X_new[:, i] for i in range(n_features)}
data_dict['Predicted_Booking_Price'] = y_pred_linear

predicted_data = pd.DataFrame(data_dict)

print("\nPredicted Booking Prices:")

print(predicted_data)
