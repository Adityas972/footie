The models selected Linear Regression and Random Forest (Spark) were chosen for the following reasons:

To compare computational performance between a fast (Linear Regression) and a slower, more complex (Random Forest) model.
To evaluate differences in results between models that are sensitive to bias and those that are more resistant to it.
Hyperparameter tuning was performed using grid search with the following values:

Linear Regression (Spark ML) regParam: [0, 0.01, 0.1, 1] maxIter: [30, 50, 70, 100]

Random Forest (Spark ML) numTrees: [5, 15, 30, 50] maxDepth: [3, 5, 10, 15]


Similarly, for the Neural Network (NN) architectures, both shallow and deep (Pytorch) networks were implemented to compare their performance and assess the performance gain achieved by increasing network depth.

Shallow Neural Network (in_dim → 16 ReLU → 1)

Deep Neural Network (in_dim → 64 ReLU → 32 ReLU → 16 ReLU → 1)
