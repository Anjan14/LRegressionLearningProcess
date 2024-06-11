# CSC 736 - Machine Learning 
## Objective
1. In this project, we will utilize knowledge of Linear Regression.  
2. Simultaneously, we will visualize the learning process of Regression.

A linear regressor is able to predict values with given inputs based on provided training
dataset. In this assignment, we are required to develop a program that is able to:  
1. Generate points in the training set.  
   i. We will arbitrarily define a line y = wx + b (e.g., y = 2x + 3) as our ground truth line.  
   ii. Generate 20 random data points (randomly select 20 x and calculate 20 y accordingly) from
       the line defined above. The y value on each point needs to randomly add or minus a noise
       with the range of 10% * y. For example, assuming our line is y = 2x + 3, our first point
       is x = 10, y = 23 + rand(23 * 0.1) or y = 23 - rand(23 * 0.1).  
   iii. Visualize the line in green and the 20 points (filled circles) on a graphic user
        interface similar to the attached figure.
   
2. Implement a linear regression with the gradient descent learning algorithm.  
   i. Randomly initialize the weight and bias to a double within (0,1).  
   ii. Set our learning rate to, (eta)η = 0.000001.  
   iii. Then we train our linear regressor by the gradient descent learning algorithm with the
        provided training data generated from the previous step.
        - Define "epoch" as one iteration of training all 20 points one time.
        - For each epoch, iterating through 20 training points (xˆi, yˆi):
          * We will use our linear model to calculate yi = wxˆi + b  
          * Calculate the accumulated error for bias:  
                   err-b = (1/m) ∑_(i=1)^m(yˆi - yi)  
          * Calculate the accumulated error for weight: err-w = (1/m) ∑_(i=1)^m [(yˆi - yi) * xˆi]
        <img width="432" alt="Screenshot 2024-06-11 at 5 07 47 PM" src="https://github.com/Anjan14/LRegressionLearningProcess/assets/89369454/b291da63-1612-450e-9bc9-33e6d5b7878d">    
   
      - Using this formula, we need to update the bias: b = b + (eta)η * error-b  
      - Using this formula, we need to update the weight: w = w + (eta)η error-b
   iv. We will visualize the line represented by the current weights at the end of 
       each epoch on GUI. (like an animation.)  
   v. Output the number of mean square error on the training data at the end of each 
      epoch  
   vi. Train our linear regression model for at least 500 epochs.

## Results and Analysis

          
         

