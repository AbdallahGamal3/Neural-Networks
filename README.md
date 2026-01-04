# Neural Networks: MLP Optimization & Regularization

## 📌 Project Overview
This repository contains a comprehensive implementation of a **Multi-Layer Perceptron (MLP)** to classify handwritten digits from the **MNIST** dataset. The project focuses on the practical application of Neural Network foundations, specifically **Optimization** strategies and **Regularization** techniques to prevent overfitting.

##  Key Experiments
This project goes beyond basic implementation by rigorously testing hyperparameters:

### 1. Optimization Algorithms
Compared convergence speed and stability across:
- **SGD** (Stochastic Gradient Descent)
- **SGD + Momentum**
- **Adam** (Adaptive Moment Estimation)
- **AdamW** (Adam with Weight Decay)

### 2. Regularization Techniques
- **Dropout:** Analyzed rates of 0.0, 0.1, 0.3, and 0.5.
- **L2 Regularization:** Tested weight decay penalties.
- **Early Stopping:** Implemented to automatically halt training when validation loss plateaus.

### 3. Hyperparameter Tuning
- **Batch Sizes:** 32 vs 64 vs 128 vs 256.
- **Activation Functions:** ReLU, Tanh, Sigmoid, GELU.

## 📊 Results Summary
| Experiment | Best Configuration | Accuracy |
| :--- | :--- | :--- |
| **Best Model** | 2 Layers + Dropout (0.1) | **99.12%** |
| **Optimizer** | AdamW | Fast Convergence |
| **Batch Size** | 32 | Best Generalization |
| **Activation** | ReLU / GELU | Highest Accuracy |

> **Note:** The project includes a custom generalization test where the model successfully predicts a hand-drawn digit ('7') that was preprocessed with Gaussian Blur to match the training distribution.

## 📂 Repository Structure
```text
Neural-Networks-MLP/
│
├── Neural_Networks_MLP_Optimization.ipynb  # The Master Notebook
├── models/                                # Saved .keras models for all experiments
├── results/                               # Generated plots and visualizations
│   ├── activation_tests/                  # ReLU vs Tanh vs Sigmoid vs GELU
│   ├── batch_tests/                       # Batch size impact (32–256)
│   ├── loss_curves/                       # Dropout and Regularization plots
│   ├── optimizer_tests/                   # SGD vs Adam comparisons
│   └── predictions/                       # Prediction samples and Custom Digit test
├── submission/                            # Detailed theoretical analysis (Markdown)
├── requirements.txt                       # Dependencies
└── README.md                              # Documentation
```
🛠️ Installation & Usage
1. Clone the repository
git clone https://github.com/YOUR_USERNAME/Neural-Networks-MLP-Optimization
cd Neural-Networks-MLP-Optimization

2. Install dependencies
pip install -r requirements.txt

3. Run the notebook
Open Neural_Networks_MLP_Optimization.ipynb using VS Code or Jupyter Lab and run all cells.

Author
Abdallah Gamal
Digital Egypt Pioneers Initiative (DEPI)
