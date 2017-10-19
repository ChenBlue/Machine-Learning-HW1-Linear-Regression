# HW1: Linear Regression
This is the homework from CS5651 Machine Learning in National Tsing Hua University.

### Instruction
Implenment Linear Regression to predict $\hat{y}$ by Tensorflow. The dataset and label are given and we have to split the data to two parts: training and testing. Head 90% are for training dataset, the others are testing dataset. After prediction, calculate the error rate to examine its performance.

### Algorithm
#### Linear Regression
$\hat{y}$ is the value we predict for y. We define the ourput is 
$$\hat{y}=XW+b ...(1)$$ 
X is a n*m input matrix. (n: number of samples, m: number of features)\\
W is a m*1 matrix, which is the linear regression parameters that we want.\\
Modify equation (1) to
$$\hat{y}=XW ...(2)$$ 
by augmenting X to n*(m+1) matrix. The last column are all one, and W will also become (m+1)*1 matrix. The last element of W achieve the same result as b. </b>
Next, apply **normal function** to derive W.
$$W=(X\^{(train)T}X\^{(train)})\^{-1}X\^{(train)T}y\^{(train)}$$
<\b>

#### Error rate
For **error rate**, it is the average of $\frac{|y-\hat{y}|}{y}$

#### Data Preprocess
Do normalization and take logarithm
$$New data=log[(data-min+1)/(max-min)]$$
"Plus 1" is because of avoiding 0 value in logarithm.

