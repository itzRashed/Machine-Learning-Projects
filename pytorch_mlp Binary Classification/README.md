# 🧠 pytorch_mlp Binary Classification
This project demonstrates how to build, train, and evaluate a simple **Multi-Layer Perceptron (MLP)** for binary classification using **PyTorch** and **scikit-learn**.

> 🚀 A great starting point to understand neural networks and deep learning fundamentals using synthetic datasets!

## 🔍 Overview
This code walks through:
- Generating synthetic binary classification data
- Defining a custom **MLP** class with PyTorch
- Training the model using **CrossEntropyLoss** and the **Adam optimizer**
- Evaluating model accuracy on a test set

## 📦 Imports Used
- `torch`, `torch.nn`, `torch.nn.functional`, `torch.optim` – Deep learning components
- `numpy` – Numerical operations
- `sklearn.datasets`, `model_selection`, `preprocessing` – Data creation and processing
- `torch.utils.data` – DataLoader and TensorDataset for efficient batch handling

## 🏗️ MLP Architecture
```python
class MLP(nn.Module):
    def __init__(self, input_size, hidden_size, output_size):
        super(MLP, self).__init__()
        self.fc1 = nn.Linear(input_size, hidden_size)
        self.relu = nn.ReLU()
        self.fc2 = nn.Linear(hidden_size, output_size)

    def forward(self, x):
        x = self.fc1(x)
        x = self.relu(x)
        x = self.fc2(x)
        return x

🧪 Training and Evaluation
🔁 train_model()
Trains the model on batches of training data using a defined number of epochs.

📊 evaluate_model()
Evaluates model performance on the test data and prints accuracy.

🧬 Main Workflow
1. Generate synthetic classification data using make_classification()
2. Split into train/test sets using train_test_split()
3. Scale features with StandardScaler
4. Create DataLoader instances for mini-batch training
5. Initialize the MLP model with specified dimensions
6. Train the model using Adam optimizer and CrossEntropyLoss
7. Evaluate model accuracy on test set

🧠 What I Learned
- How to build a basic feedforward neural network using PyTorch
- How to preprocess data and handle batches efficiently
- How to apply model evaluation using test accuracy

📜 License
This project is licensed under the MIT License – use, modify, and share freely.
