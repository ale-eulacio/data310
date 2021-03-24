For my project I chose Colombia. I initially wanted to do the project on Venezuela but the DHS does not conduct surveys there. There were about 44,000 housholds worth of
data, with around 162,000 individual persons

PENALIZED REGRESSION MODEL

Question #1 - Which "top_model" performed the best?

INSERT SC OF SLICES LIST HERE

For the 15 slices taken, the mean AUC ranged from 0.633 to 0.621. The first five slices had an AUC of of 0.633, making them the best peforming models. The model that seemed to 
be most succesful, however, was model 5. This is because it was the most penalized but it still had the highest AUC score of the bunch.

INSERT LR PLOT HERE

Question #2 -  Are you able to use the feature selection penalty to tune your hyperparameter and remove any potentially irrelevant predictors?

Yes, I used feature selection penalty to select model 5 as the best one. Regardless of the fact that model 5 was more penalized than models 1-4, it kept the same AUC score as
the others. This means that this model was able to get rid of irrelevant predictors while maintaining the same AUC score, making it a better performer than the first 4. I think 
the argument could be made that models 6-10 could also be considered succesful. They were only .001 and .002 away from the original AUC, but were even more penalized. Hwoever, I
ended up sticking with number 5 because it had the highest AUC

Question 3 - Provide your ROC plots and interpret them. How effective is your penalized logistic regression model at predicting each of the five wealth outcomes.

INSERT ROC PLOTS HERE

The model is very effective at predicting the 1st and 5th wealth outcomes. This is to be expected, because the two extremes are the easiest to differentiate. I was surprised to 
find that wealth classification number 1 was the second largest subset of the data (27% of the data). I imagine that the model found patterns in specific predictors like education
level or size of household that helped differentiate class 1 regardless of its size. I think that the the model did struggle with the size of wealth class 2 (28% of all data).
This is where the model performed the worst, and I imagine that there were a great range of values for the predictors in this wealth class. This would make it extremely difficult
for the model to find any patterns and have any predictive power. The same goes for class 3. I imagine that class 5 has discernable patterns in its predictor values that helped 
the model clearly differentiate this class from the other 4. 

RANDOM FOREST
