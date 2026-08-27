# Experiment 2 — Comparative Study of Activation Functions and Optimization Algorithms in Deep Learning

## Student Details

**Name:** Mohamed Aashik S  
**Roll No:** 24BAD072  

---

## Experiment Overview

This experiment focuses on comparing different activation functions and optimization algorithms used in deep learning. The main objective is to understand how activation functions affect neural network learning and how different optimization algorithms influence convergence, loss, and accuracy.

The experiment also demonstrates how Google Colab, Google Drive, and GitHub can be used to organize, store, document, and manage deep learning experiments.

---

## Objectives

- Understand the role of activation functions in neural networks.
- Visualize and compare Sigmoid, Tanh, and ReLU.
- Evaluate the performance of different activation functions in an ANN.
- Compare different gradient-based optimization algorithms.
- Analyze optimizer convergence and model accuracy.
- Learn experiment management using Google Colab and Google Drive.
- Maintain reproducible experiments using GitHub and version control.

---

## Tools and Technologies

- Python
- TensorFlow
- NumPy
- Matplotlib
- Google Colab
- Google Drive
- GitHub

---

# Task A — Visualization of Activation Functions

The first task visualizes and compares three commonly used activation functions:

1. Sigmoid
2. Tanh
3. ReLU

The functions are plotted over a range of input values to study their output behavior.

### Comparison

| Activation Function | Output Range | Main Characteristic |
|---|---|---|
| Sigmoid | 0 to 1 | Smooth function with saturation |
| Tanh | -1 to 1 | Zero-centered and smooth |
| ReLU | 0 to infinity | Simple and computationally efficient |

The experiment also considers saturation regions, gradient behavior, computational efficiency, and typical applications of the three functions.

---

# Task B — Performance Comparison of Activation Functions

An identical Artificial Neural Network architecture is trained using:

- Sigmoid
- Tanh
- ReLU

The same dataset, model structure, optimizer, number of epochs, and validation split are used so that the activation functions can be compared fairly.

The following performance measures are recorded:

- Training accuracy
- Validation accuracy
- Training loss
- Validation loss
- Convergence behavior

Graphs are generated to compare validation accuracy and validation loss across epochs.

### Expected Observation

ReLU generally provides efficient training because it avoids saturation for positive inputs and maintains a useful gradient. Sigmoid and Tanh may experience slower learning when their neurons enter saturation regions.

The final conclusion should be based on the actual results obtained during the experiment.

---

# Task C — Comparison of Optimization Algorithms

The same ANN architecture is trained using four optimization algorithms:

1. SGD
2. Momentum
3. RMSProp
4. Adam

The optimizers are compared using:

- Training loss
- Validation loss
- Convergence speed
- Final training accuracy
- Final validation accuracy

The experiment generates:

- Training Loss vs Epoch
- Validation Loss vs Epoch
- Validation Accuracy vs Epoch

### Expected Observation

SGD provides basic gradient-based optimization but may converge more slowly. Momentum improves SGD by using information from previous updates. RMSProp adapts the learning rate for different parameters. Adam combines adaptive learning rates with momentum-based updates and commonly provides fast convergence.

The actual graphs and recorded results are used to determine the best optimizer for the experiment.

---

# Task D — Deep Learning Experiment Management

This task demonstrates the use of cloud storage and version control for managing deep learning experiments.

### Google Colab

Google Colab is used as the development and execution environment for the Python and TensorFlow code.

### Google Drive

Google Drive is mounted in Colab to store:

- Experiment notebooks
- Trained models
- Experiment results
- Other related files

### GitHub

GitHub is used for:

- Storing the experiment notebook
- Maintaining source-code versions
- Recording changes through commits
- Sharing the project
- Supporting reproducibility and collaboration

---

## Project Structure

```text
EX2-Deep-Learning-Comparative-Study/
│
├── EX2_Comparative_Study_All_Tasks_24BAD072.ipynb
├── README.md
│
├── models/
│   ├── relu_activation_model.keras
│   └── adam_optimizer_model.keras
│
└── results/
    ├── activation_comparison
    └── optimizer_comparison