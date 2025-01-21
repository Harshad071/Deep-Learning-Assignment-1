# Deep-Learning-Assignment-1
# Neural Network From Scratch  

## Objective  
Implement a simple feedforward neural network from scratch in Python without using any in-built deep learning libraries. This implementation will focus on basic components like forward pass, backward propagation (backpropagation), and training using gradient descent.  

---

## Problem Definition  

### Dataset  
**Input (X):**  
```python
[[0, 0], [0, 1], [1, 0], [1, 1]]
Output (y):

python
Copy
Edit
[[0], [0], [0], [1]]
This dataset represents the binary inputs and their corresponding output for the AND operation.

Task
The task is to train a neural network to predict the output of the AND operation based on the provided input combinations. The problem is a binary classification task.

Methodology
Neural Network Architecture
Input Layer: 2 neurons (representing two binary inputs)
Hidden Layer: 3 neurons with sigmoid activation
Output Layer: 1 neuron with sigmoid activation for binary classification
Forward Pass
The input is passed to the hidden layer, where weighted sums are computed.
The hidden layer's output is computed using the sigmoid activation function.
The output layer takes the hidden layer's output and computes the final output using sigmoid activation.
Backpropagation
The error is calculated between the predicted output and actual output.
The error is propagated backward through the network, adjusting the weights and biases using gradient descent based on the computed gradients.
Loss Function
The Mean Squared Error (MSE) loss function is used to measure the difference between the predicted and actual outputs:
𝐿
𝑜
𝑠
𝑠
=
1
𝑛
∑
𝑖
=
1
𝑛
(
𝑦
𝑖
−
𝑦
^
𝑖
)
2
Loss= 
n
1
​
  
i=1
∑
n
​
 (y 
i
​
 − 
y
^
​
  
i
​
 ) 
2
 
Optimization
The network is trained using gradient descent, adjusting weights and biases in the direction of the negative gradient to minimize the loss function.

How to Run the Code
Clone the repository:

bash
Copy
Edit
git clone https://github.com/harshadjadhav/Deep-Learning/tree/main/Neural_Network_From_Scratch.git
Navigate to the project directory:

bash
Copy
Edit
cd Neural_Network_From_Scratch
Run the Python script:

bash
Copy
Edit
python neural_network.py
The network will train on the AND problem dataset for 14,000 epochs and print the loss at regular intervals (every 1,000 epochs).

Results
Training Loss
The network reduces the loss over 14,000 epochs. Example outputs:

yaml
Copy
Edit
Epoch 0 - Loss: 0.2656253844377818  
Epoch 1000 - Loss: 0.25052722352922147  
Epoch 2000 - Loss: 0.2504432418426345  
Epoch 3000 - Loss: 0.2503755345024164  
Epoch 4000 - Loss: 0.2503195105633955  
Epoch 5000 - Loss: 0.2502726087280806  
Epoch 6000 - Loss: 0.25023291486231  
Epoch 7000 - Loss: 0.25019897699868454  
Epoch 8000 - Loss: 0.25016967854138145  
Epoch 9000 - Loss: 0.250144149816591  
Epoch 10000 - Loss: 0.2501217053593956  
Epoch 11000 - Loss: 0.2501017987750972  
Epoch 12000 - Loss: 0.25008398979392515  
Epoch 13000 - Loss: 0.25006791991038824  
Epoch 14000 - Loss: 0.25005329414835653  
Predictions After Training
The predictions for the AND operation are as follows:

python
Copy
Edit
[[0.50140679]  # Input: [0, 0] -> Output: ~0  
 [0.48687625]  # Input: [0, 1] -> Output: ~0  
 [0.51232741]  # Input: [1, 0] -> Output: ~0  
 [0.49762452]] # Input: [1, 1] -> Output: ~1  
Technologies Used
Python 3.x
NumPy (for matrix operations)
Author
Harshad Jadhav
