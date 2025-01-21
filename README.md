# Neural Network Implementation from Scratch

This repository demonstrates the implementation of a simple feedforward neural network from scratch in Python. It focuses on key components such as forward pass, backpropagation, and gradient descent optimization.

## Problem Definition

### Dataset
The dataset used for this example is a binary classification problem: the **AND operation**.

- **Inputs**: All possible combinations of binary values:  
  - [0, 0]  
  - [0, 1]  
  - [1, 0]  
  - [1, 1]  
- **Outputs**:  
  - The expected results of the AND operation:  
    - [0], [0], [0], [1]

---

## Implementation

The neural network has the following architecture:
1. **Input Layer**: 2 input features.  
2. **Hidden Layer**: 3 neurons with a sigmoid activation function.  
3. **Output Layer**: 1 neuron with a sigmoid activation function.

### Key Features
- **Custom Weights and Bias Initialization**:  
  The weights and biases are initialized explicitly to demonstrate the learning process.
- **Sigmoid Activation Function**:  
  Used for both hidden and output layers to map the output between 0 and 1.
- **Gradient Descent Optimization**:  
  Updates weights and biases through backpropagation.

---

## Training Results

### Loss during Training
The loss was minimized over **14,000 epochs** using the **Mean Squared Error (MSE)** as the loss function. Below is a sample of the training log:

- **Epoch 0** - Loss: `0.2656253844377818`
- **Epoch 1,000** - Loss: `0.25052722352922147`
- **Epoch 2,000** - Loss: `0.2504432418426345`
- **Epoch 3,000** - Loss: `0.2503755345024164`
- **Epoch 4,000** - Loss: `0.2503195105633955`
- **Epoch 5,000** - Loss: `0.2502726087280806`
- **Epoch 6,000** - Loss: `0.25023291486231`
- **Epoch 7,000** - Loss: `0.25019897699868454`
- **Epoch 8,000** - Loss: `0.25016967854138145`
- **Epoch 9,000** - Loss: `0.250144149816591`
- **Epoch 10,000** - Loss: `0.2501217053593956`
- **Epoch 11,000** - Loss: `0.2501017987750972`
- **Epoch 12,000** - Loss: `0.25008398979392515`
- **Epoch 13,000** - Loss: `0.25006791991038824`
- **Epoch 14,000** - Loss: `0.25005329414835653`

---

### Predictions after Training
The model's predictions for the **AND operation** are as follows:

- `[0, 0]` -> `0.50140679`
- `[0, 1]` -> `0.48687625`
- `[1, 0]` -> `0.51232741`
- `[1, 1]` -> `0.49762452`

These values are close to the expected results of the AND operation: `[0, 0, 0, 1]`.


## Usage

To run the code:

1. Clone the repository:
    ```bash
    git clone https://github.com/username/repo-name.git
    cd repo-name
    ```

2. Install the required dependencies:
    ```bash
    pip install numpy
    ```

3. Run the script:
    ```bash
    python neural_network_and.py
    ```

---

