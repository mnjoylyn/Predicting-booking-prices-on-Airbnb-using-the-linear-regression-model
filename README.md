# Predicting-booking-prices-on-Airbnb-using-the-linear-regression-model
Let’s say we want to build a model to predict booking prices on Airbnb. Between linear regression and random forest regression, which model would perform better and why?
import numpy as np
import pandas as pd
# Data for prediction
n_samples = 5  # You can adjust the number of samples
n_features = 5

# Generate random features (e.g., location, property size, amenities, etc.) for prediction
X_new = np.random.rand(n_samples, n_features)
print("New Data for Prediction (X_new):")
print(X_new)

# The Linear Regression model
y_pred_linear = linear_reg.predict(X_new)

# DataFrame to display the predictions alongside the features
data_dict = {f'Feature_{i}': X_new[:, i] for i in range(n_features)}
data_dict['Predicted_Booking_Price'] = y_pred_linear
predicted_data = pd.DataFrame(data_dict)

# Predicted data
print("\nPredicted Booking Prices:")
print(predicted_data)
