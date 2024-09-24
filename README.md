# Soccer-RandForestPredictor

This Google CoLab entry imports a CSV web scraped data from several seasons of Premier League soccer matches. The code then cleans the data, creates columns of predictors of the cleaned data (changed non-int types to parsable features for the Random Forest Model)

Then, a Random Forest Model is imported and initialized. The data is split between training and testing based on the date (all training data's date being before the test data)

The Random Forest Model is then fit unto the training dataset with the specific column predictors, and predictions are made. Then the accuracy metric is used with a confusion matrix. The precision score is particulary low so additional predictor vectors are calculated by group with the rolling_averages(). A compact prediction function is then made. Lastly, a dictionary is made to fill and match related team names across the soon the be merged dataframes.
