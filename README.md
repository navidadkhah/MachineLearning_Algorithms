# Machine Learning
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
    <img alt="Min Samples Leaf" src="https://github.com/user-attachments/assets/018aa5b4-35b2-4a50-ab76-c16e6c82cc4c" width="400">
    <img alt="Max Depth" src="https://github.com/user-attachments/assets/605fb2eb-c6c2-474e-904c-9f5834ec9cbf" width="400">
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


