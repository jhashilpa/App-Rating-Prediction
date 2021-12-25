The aim of the project is to create a ML model which can predict the rating of an app based on characteristics like No. of reviews,No. of times app is downloaded, Price, type & Category of app ,
supported android version ,last updated date etc.

1>Data Cleaning is done as there were lot of alphanumeric charcaters present in columns such as Price, No of times app was downloaded and No of reviews.

2>There were huge number of levels present in features like Category and supported Android versions.Instead of creating dummy variables for all the lables top 10 most 
frequent labels for each predictor is calculated and dummy variable are created for only those frequent labels. This approach prevents curse of dimensionality.

3>Data Scaling is being implemented as feature data is collected at different scales. For ex. No of reviews is in 1000's,and Price is in 100's.

4>ExtraRegressor,Random Forest Regressor and KNN regressor model are created. As the dataset has many outliers,We chose these model as they are not very much sensitive to outliers.

5>The model is saved in pickle format and can be used in predictions in future
