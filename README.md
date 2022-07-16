# flight-price-prediction
- Initially the training data is loaded into dataframe using pandas framework and then data is handled for any missing values that are present in the data.
- Data from features like Date_of_Journey, Dep_Time, Arrival_Time is extracted using to_datetime function via pandas framework.
- Categorical features like Airline, Source, Destination are converted to numeric using OneHotEncoder and feature called TotalStops is converted to numeric using Label Encoder.
- Feature selection is carried out by plotting correlations between different features in form of heatmap using seaborn plot.
- An Extra Tree Regressor was built on top of this data to extract important features among all available independant features.
- Logistic Regression model was built on this selected data where parameters of the model were tuned by RandomizedSearchCV. The model RMSE score on the test dataset was found to be 4303.57.
- Similarly, random forest model was built on the training data and this model produced RMSE score of 1759 on the test dataset indicating that it is the better model among the two built models for this dataset.  
