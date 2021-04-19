Like I am sure most other people in the class did, I am using the linear regression and random forest models to predict population values at 100X100 meter grid cells in my chosen country. I ended up having to change my chosen country because of the size of the vector file of Colombia, my original country. Because it was too large, I ended up staying in the area and chose the Dominican Republic as my country due to the much smaller size. Here, I was actually able to develop some pretty solid results for the two models using the dasymetric allocation. Here are some graphs and numbers to visualize how these models did. 

LINEAR REGRESSION MODEL

First, the difference in between the predicted populations sum and the real number was pretty close for this for how simple of a model it is. It overpredicted by 622,458 (12,073,435[actual pop] - 12,080,977[predicted pop]). For the margins that we are working in, half a million is not that bad considering the simplicity of the model. The difference in sums was also pretty solid, with the error ranging from -146 to 84. Here are some graphs to help visualize the results.

Population Sums plot
 
INSERT POP_SUMS_PLOT

Difference of Sums plot

INSERT DIFF_SUMS_PLOT HERE

3D positive side (areas with large population) Predicted Values

INSERT 3D POSITIVE SIDE

3D negative side Predicted Values

INSERT 3D NEGATIVE SIDE 
`
MSE

INSERT HERE

ME 

INSERT HERE

Random Forest Model

The difference in total sums for the random forest model was even better than the Linear regression model. The Random forest model underpredicted by 551,321 (12,624,756[actual pop] - 12,080,977[predicted pop]). I don't think it matters if the prediction is over or under, and because of this the absolute value means that the Random forest model performed better! The MSE graph also helps to show this. 

Population Sums plot
 
INSERT POP_SUMS_PLOT

Difference of Sums plot

INSERT DIFF_SUMS_PLOT HERE

3D positive side (areas with large population) Predicted Values

INSERT 3D POSITIVE SIDE

3D negative side Predicted Values

INSERT 3D NEGATIVE SIDE 

MSE

INSERT HERE

ME 

INSERT HERE
