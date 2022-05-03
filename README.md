COLLABORATIVE FILTERING USING THE NETFLIX DATA


***Motivation:
To recommend recommendation with user based movie recommendation.

Alternating Least Squares (ALS) is collaborative filtering method for recommender systems.

Pearson Correlation Coefficient (PCC) is one of the most popular similarity measures for Collaborative filtering recommender system, to evaluate how much two users are correlated. 

Dataset [TrainingRating, TestingRating and Movies] which has data UsedId, MovieId, Rating and Movie name.


***Step1
 First I load three of datasets, namely movie, train and test rating in spark environment.
 
 
***Step2
 Data preprocessing
 Build an ALS model based by tuning parameters (maxIter, rank, regParam) to obtain the 
model with the smallest RMSE on the validation set. 


***Step3
 By the best model obtained from the above step, making predictions of ratings on movies in 
the test set and calculating the RMSE to evaluate the model performance are preparing for 
the next step.


***Step4
 In this step, I use the prediction results by the best model to recommend movies for random 
userID 1744889


***Conclusion
The RMSE of the best ALS model on the test data is 0.83896, indicating the model is with good perf
ormance in predicting the ratings for movies
