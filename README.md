# Projects

Logistic Regression

Implement 2-class logistic regression using gradient descent as outlined in the lecture notes. You can do either batch or stochastic versions of the algorithm. You will only use your algorithm for this dataset, so you can hard-wire in the number of instances and the size of each instance. The goal is not to write a generic version of the algorithm (though you can if you wish). The goal is to understand how it works on real data.

Use your algorithm to learn a classifier that determines whether an input image is an 8 or one of the other digits and record the classification accuracy on the training set (the full dataset I provided). Note that you'll have to come up with some stopping criterion, which could be to simply run for a fixed number of iterations and then quit.

After training is complete, create a 28x28 image of the learned weights. The largest weight (most positive) should map to black, the smallest weight (most negative) to white, and the other weights should linearly interpolate between those extremes.

Recall from class that one form of regularization (a way to prevent overfitting) is to encourage the weight vector to be sparse. That is commonly done in logistic regression by adding a term to the objective function that is the sum of the squares of the individual weights. We'd like to minimize that while maximizing the likelihood of the data.

Modify your code from above to include this term. Note that you'll have to consider the derivative of this term when computing gradients, and the formulation in class is maximizing likelihood whereas we want to minimize the sume of squared weights. Introduce a parameter, lambda, that is a constant used to multiply the sum of squares of weights. If lambda = 0, then you are running logistic regression without regularization. If you increase lambda, then you are putting more emphasis on small weights.


Data Set :
http://yann.lecun.com/exdb/mnist/

