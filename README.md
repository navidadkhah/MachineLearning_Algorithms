# Machine Learning Algorithms
In this repository, I implemented Supervised and Unsupervised algorithms. 
- Supervised algorithms contain KNN, SVM, Decision Tree and, type of Regression.
- Unsupervised contains DBSCAN, an algorithm for clustering.<br>

First of all, I describe Supervised algorithms and then, Unsupervised:
## Decision Tree
In the notebook, In part B, I implemented the Decision Tree Algorithm and changed Hyperparameters such as ```Max Depth``` and ```Min Samples Leaf```:
 <table>
  <tr>
    <th>Max Depth</th>
    <th>Min Samples Leaf</th>
  </tr>
  <tr>
    <td>It Determines the maximum depth or level of the tree. It controls the number of splits or decision nodes in the tree.</td>
    <td>
    It specifies the minimum number of samples required to be at a leaf node. 
    A leaf node is a node that does not split further and represents a final decision or prediction.
     </td>
  </tr>
</table> 



<p align="center">
    <img alt="Max Depth" src="https://github.com/user-attachments/assets/605fb2eb-c6c2-474e-904c-9f5834ec9cbf" width="400">
    <img alt="Min Samples Leaf" src="https://github.com/user-attachments/assets/018aa5b4-35b2-4a50-ab76-c16e6c82cc4c" width="400">
</p>

In each situation, I have changed ```Learning Rate``` and plotted it to find the best number of the Hyperparameters.<br>
In part C, I trained data using ``` RANDOM FOREST``` and ```Gradient Boosting```. Finally, I plotted the Learning Curve for each one.
> Between these three algorithms, ***Random Forest*** and ***Gradient Boosting*** have higher Test Score.
<p align="center">
    <img alt="Gradient Boosting" src="https://github.com/user-attachments/assets/e64fcf9a-3095-4754-bc6f-7cae48edb081" width="330">
    <img alt="Random Forest" src="https://github.com/user-attachments/assets/d046d361-b6c9-4240-b4dc-35dd8c52c673" width="330">
    <img alt="Decision Tree" src="https://github.com/user-attachments/assets/b05c376f-212b-497d-a246-969c5699b75f" width="330">
</p>

- Also, you can find the Dataset as a `numpy` file and use it for your project.

## KNN
Implement the K-Nearest Neighbors (KNN) algorithm from scratch on the Disease dataset. The model's accuracy on the test data is reported using the functions from the Scikit-learn library. The ROC curve for the Trained KNN model is plotted. The ROC (Receiver Operating Characteristic) curve is a graphical plot that illustrates the diagnostic ability of a binary classifier system as its discrimination threshold is varied.
First of all, We need to preprocess our data. After that, we implemented ```KNN``` from scratch and split train and test data.

<p align="center">
   <img alt="ROC Plot" src="https://github.com/user-attachments/assets/8f20038d-8e6e-4d36-be5d-64454f52518c" width="400">
</p>

The ROC plot is used to determine how much our model predicted well. The closer the AUC is to 1, the better the model's performance.

## SVM
SVM or Support Vector Machine is a Supervised learning algorithm used for both classification and Regression. In SVM, our goal is to find the best decision boundary for separating classes. Now, we have a dataset. it describes pieces of information about the history of strokes between 43400 people.
The whole steps are as follows:
- Reading the ```csv``` dataset.
- Feature Engineering such as filling null rows and one hot their columns.
- Normalize the data.
- Splitting train and test data.
- Now, we are checking about data balancing, To fix this problem, we use the ```Data Augmentation `` method.
- Creating a model with its associated library.
- Plot ROC and Confusion Matrix.

  <p align="center">
   <img alt="ROC Plot" src="https://github.com/user-attachments/assets/9196e99d-63d2-4901-b000-7a99bf1d5527" width="400">
   <img alt="Confusion Matrix" src="https://github.com/user-attachments/assets/281fb22d-ad0a-4879-a050-3f2245ef9819" width="400">
  </p>

> Note: In the Confusion Matrix, we try to increase True-Positive and True-Negative.


## Polynomial Regression
In this assignment, we have insurance information and we want to implement a regression model.<br>
First of all, we start with preprocessing and use the one-hot encoder for columns. we plot the regression line for the three train-test-split sizes and we realize the best size for it is 80 percent because it reduces the cost. In the end, we measure MSE and R-squared:
<img alt="plot" src="https://github.com/user-attachments/assets/7e13e9f6-23b9-4742-8d27-89c607db8ee8" width="600">
<img alt="Messure" src="https://github.com/user-attachments/assets/7ed2fad7-c05c-4843-aa8a-603c82507f3e" width="300">




Now, we want to increase the accuracy. For this, we use Polynomial Reggresion. we add ```bmi^2``` column to the dataset.<br>
The result is as follows:
<br>
<img alt="plot" src="https://github.com/user-attachments/assets/a2ffa8e7-029c-49ac-953d-cbad20cfb7ba" width="600">
<img alt="Messure" src="https://github.com/user-attachments/assets/d043859b-3b8d-4d68-8f0d-06886d75ef99" width="300">

If we compare these together, we realize that when we add a polynomial feature, we have a better model. our R-squared ***increased*** and MSE ***decreased*** which is good.

## DBSCAN
Finally, DBCSAN or density-based clustering non-parametric algorithm is an Unsupervised Algorithm. In this algorithm, we cluster classes with some techniques.
Firstly, we initialize two hyperparameters, ```eps``` and  ```min_samples```.<br>
These hyperparameters, determine the distance of points to each other and the number of minimum samples we want to find. with these two, we can find different clusters and noise.<br>
We have two datasets that we want to cluster.
- In the first dataset, we have two clusters which are yellow and green with purple noises:

  <img alt="plot" src="https://github.com/user-attachments/assets/663b0f49-9e99-4361-b3f6-1d5eb710ac96" width="400">
  <img alt="plot" src="https://github.com/user-attachments/assets/70cf996d-8b1d-4343-b2c0-15d43f8d6925" width="400">

- In the second dataset, we have two clusters which are yellow:

  <img alt="plot" src="https://github.com/user-attachments/assets/73105ceb-6a14-4d00-9a6d-99dd23b2e204" width="400">
  <img alt="plot" src="https://github.com/user-attachments/assets/d6e04f0f-9465-4d3a-806b-acbb614be6ab" width="400">
