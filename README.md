# zillow-project
Project: Single family residence price.

## Project Goal
Build the machine learning model that can predict single family residence prices based on the data from 2017.

## Our Plan

#### Aqcuire and prepare
* Acquire the data from the zillow database. Transform the data to a Pandas dataframe to make it easy to use and manipulate in the Jupyter Notebook.
* Prepare the data for exploration and analysis. Find out if there are some values missing and find a way to handle those missing values.
* Change the data types if needed
* Find if there are features that can be created to simplify the exploration process.
* Handle the outliers.
* Create a data dictionary.
* Split the data into 3 data sets: train, validate and test data (56%, 24%, and 20% respectively)
* 'taxvaluedollarcnt' was changed to 'home_value'

#### Explore
* Explore the train data set through visualizations and statistical tests.
* Find which features have an impact on the house prices.
* Make the exploration summary and document the main takeaways.
* Impute the missing values if needed.
* Pick the features that can help to build a good prediction model.
* Identify if new features have to be created.
* Encode the categorical variables
* Split the target variable from the data sets.
* Scale the data prior to modeling.


#### Build a Model
* Pick the regression algorithms for creating the prediction model.
* Create the models and evaluate regressors using the RMSE score on the train data set.
* Find out which model has the best performance: relatively high predicting power on the validation set and slight difference in the train and validation prediction results.
* Make predictions for the test data set.
* Evaluate the results.



## Data Dictionary

|Feature | Definition   |Manipulations  |  Data type | 
|---|---|---|---|
|  county_name| Names of the different counties in our data set |  'LA', 'Orange', 'Ventura' | Category  |  
| sq_feet |  Square feet of the house |  Change type to integer |  Integer |
| lot_sqft  |  Square foot of the land |  Change type to integer |  Integer |   
| house_age  | Age of the house from year built  |  Change type to integer |  Integer | 


## Takeaways

* The mean price is greater than median price by about $80K
* There is a positive correlation between square footage and price
* Gradient Boosting Regressor performed the best with our data set
* Scaling type didn't affect the regression model's performance

## Conclusion and Next Steps

* Overall my regression model performs good. Its predictions beat the baseline model by 33.1%
* For more stable results I would pick Random Forest Regressor or Lasso Lars Regressor.
* To imporove prediction results I would recommend to pull more features from the database and look for the ones that have a strong correlation with the price in LA county.
* Also I would focus on making a model that is more stable than the current.







