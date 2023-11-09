# Bulldozer-price-prediction-regression-model
The project is inspired by the Blue Book for Bulldozers competition on Kaggle.
**Problem Definition:** Given a time-series based massive dataset of Bulldozers, a model to predict the sale-price has to be built.

- The raw dataset had around 53 features and a significant amount of noise. It needed quite a lot of feature engineering and data cleaning.
- Steps followed in data preprocessing:
- 1. Parsing the dateOfSale column during the time of importing itself
  2. The parsed date column was exploited to infer the data.
  3. LabelEncoder was equipped to engineer the categorical feature.
  4. The missing values were filled using SimpleImputer. Discrete data was filled with `median' and the categorical data was filled with `mode`.
     
- RandomForestRegressor algorithm was chosen for the model development.
- The Hyperparameter tuning was carried out by RandomSearchCV.
- The final model was assigned with the best parameters.
