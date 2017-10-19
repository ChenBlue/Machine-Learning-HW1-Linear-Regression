# HW1: Linear Regression
This is the homework from CS5651 Machine Learning in National Tsing Hua University.

### Instruction
Implenment Linear Regression to predict $\hat{y}$ by Tensorflow. The dataset and label are given and we have to split the data to two parts: training and testing. Head 90% are for training dataset, the others are testing dataset. After prediction, calculate the error rate to examine its performance.

### Algorithm
##### Linear Regression
$\hat{y}$ is the value we predict for y. We define the ourput is 
$$\hat{y}=XW+b$$ 
X is the input which has n rows * m columns. n: number of samples, m: number of features.
