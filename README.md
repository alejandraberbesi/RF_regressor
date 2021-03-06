# Random Forest Regressor model

The dataset for the predictive model consisted of 4 continuous, 2 discrete and 2 categorical variables. The label was a continuous variable. Initially it had 1000 rows. 2 variables were taken only as informative (key_1 and date_2).

The data was uploaded in google drive and then imported from a comma-separated file as a dataframe.

For the cleaning process, missing values' rows found in one of the discrete variables (disc_6) and in the labels were eliminated. The dataset didn't have duplicated rows.

There were outliers found in the following variables: 'cont_3', 'cont_4' and in the label. The rows with these outliers were also deleted.

After the cleaning process there are 789 rows left in the total dataset.

A correlation analysis indicated that 'cont_9' and 'cont_10' variables were strongly correlated; 'cont_10' was eliminated from the dataset of the predictive model.

The training set consists of 75% of the dataframe rows, the validation set of 15% and the test set of 10% of the remaining rows.

The method chosen for the modeling is a Random Forest Regressor, given that it performs well with categorical and numerical variables, it is less prone to overfitting, it doesn't need huge amounts of data to produce good results and allows interpretability.

The number of trees in the forest is 300. For the calculation of the accuracy, the mean absolute percentage error (MAPE) is used.

The predictive accuracy of the model is 92.27 %. The most important feature is 'cont_9' and the least important ones are the categorical (cat_7,cat_8). 






