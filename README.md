"# DSI-Project-2" 

Content
1. Problem Statement
2. Data Inputs, Output and Dictionary
3. Modeling Process
4. Model Results
5. Inference and Conclusion

Problem Statement
1. Create a regression model to predict housing sales price
2. Build based on Ames Iowa housing dataset
3. Explore and discover which variables are the good predictors for price estimation

Data Inputs
1. train.csv
2. test.csv

Data Output
1. submission.csv

Data Dictionary
1. Link for data description: (http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)

Modeling Process
1. EDA to explore the relation between the variables and select predictors
2. Perform deductive imputation on data for selected predictors
3. Polynomial expansion on numerical features
4. One-hot encoding on categorical variables
5. Train/test split on ‘train.csv’
6. Model selection through cross-validation
7. Model fitting on entire ‘train.csv’ dataset
8. Data preparation for ‘test.csv’ dataset
9. Prediction and Kaggle submission

Model Results
1. The RMSE for the model are as follow: (i) `train.csv`: 26927 (Model Fitting score) and (ii) `test.csv`: 24662 (Kaggle score).
2. We see that the RMSE difference is less than 10% between seen and unseen data, and therefore can say that the developed model is well-fitted.

Inference and Conclusion
1. We observed that the better numerical and categorical predictors are ['Full Bath','Year Built','Total Bsmt SF','Garage Area','Gr Liv Area','Overall Qual'] and ['Foundation','BsmtFin Type 1'] respectively.
2. Surprisingly, ['Lot Size'], which is more common and intuitive, does not have a very strong relationship with SalePrice as compared to above, and did not yield good prediction results.