1. The purpose of the training set of the data is to train the computer to recognize the patterns of the clothing. It uses the training data to learn the patterns and then the testing data set is used to test how well the model performs. 
2. The softmax option is used to determine which of the 10 different numbers has the highest probability that it matches the image. Softmax automatically turns the highest probability to one and all other probabilities to 0. The relu function does almost the opposite where it automatically turns any value below 0 into 0, in order to ensure that the function runs properly. The network had 10 denses at the end that each represented one of the 10 options of clothing items. 
3. The optimizer has the job to optimize the model to be as accurate as possible, while the loss function is telling it how wrong it is through the specific measurement (MSE or SCC). The optimizer uses the loss function to keep tweaking the model until it runs as accurately as possibly. That is why the loss gets smaller and smallers as more epochs are run.
4. A. 60,000 28x28

   B. 60,000
   
   C. 10,000 28x28
   
   D. Don't know how to put images in github. I used x_test[88] which was 6, and my model predicted that correctly/
   
