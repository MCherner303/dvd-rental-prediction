# dvd-rental-prediction
 machine learning project that uses regression models to predict the number of days a customer will rent a DVD


Summary of Results and Process
This project explores predicting the number of days a customer rents a DVD using machine learning regression models. The dataset, rental_info.csv, contains information about rental dates, movie features, and pricing.

Process
Preprocessed the dataset:
Calculated rental duration (rental_length_days) using rental and return dates.
Created dummy variables for special features (deleted_scenes, behind_the_scenes).
Excluded features that leaked information about the target.
Split the data into training (80%) and testing (20%) sets, ensuring reproducibility with random_state=9.
Trained multiple regression models:
Linear Regression
Decision Tree Regressor
Random Forest Regressor
Evaluated models using Mean Squared Error (MSE) on the test set.
Results
Best Model: Random Forest Regressor
MSE: 2.03 (well below the target of ≤ 3)
This model can help optimize inventory planning by accurately predicting DVD rental durations. The trained model is saved as best_model.pkl for future use.

