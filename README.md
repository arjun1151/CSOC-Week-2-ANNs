# CSOC-Week-2-ANNs
# Neural Network from Scratch and PyTorch

A comparative implementation of a Multilayer Perceptron (MLP) for handwritten digit classification on the MNIST dataset. This project compares a neural network implemented from scratch using NumPy with an equivalent implementation using PyTorch, while evaluating the impact of framework optimizations and hardware acceleration on training performance.

## Features

- Neural Network wiht NumPy and scratch implementations
- Manual forward and backward propagation
- Gradient Descent optimization
- Performance comparison across different hardware platforms
- Confusion Matrix visualization
- Training loss visualization

## Project Structure

```
.
├── data/
│   └── mnist.zip
├── scratch/
│   ├── L_layered_NN_CSOC_Week_2 Local.ipynb
│   └── L_layered_NN_CSOC_Week_2_Colab_CPU.ipynb
├── pytorch/
│   ├── PyTorch_Implementation_CSOC_Week_2_CPU.ipynb
│   └── PyTorch_Implementation_CSOC_Week_2_GPU.ipynb
└── README.md
```

## Dataset

The project uses the **MNIST Handwritten Digit Dataset**, containing:

- 60,000 training images
- 10,000 testing images
- 10 digit classes (0–9)
- Image size: 28 × 28 grayscale

## Implementations

The following implementations are included:

1. PyTorch implementation on Colab's T4 GPU
2. PyTorch implementation on Local CPU
3. NumPy implementation on Local CPU
4. NumPy implementation on Colab CPU

## Methodology

The workflow consists of:

1. Data Loading
2. Data Preprocessing
3. Neural Network Initialization
4. Forward Propagation
5. Backpropagation
6. Model Evaluation
7. Performance Comparison

## Performance Comparison

The implementations are compared using:

- Training Time
- Peak Memory Usage
- Test Accuracy
- Convergence Speed

| Implementation | Training Time (s) | Peak Memory (MB) | Test Accuracy (%) |
|----------------|------------------:|-----------------:|------------------:|
| PyTorch (Colab GPU) | 460.01 | 1872.71 | 93.35 |
| PyTorch (Local) | 597.95 | 1218.66 | 93.54 |
| Scratch (Local) | 846.92 | 1028.67 | 94.61 |
| Scratch (Colab CPU) | 2288.18 | 1197.30 | 94.60 |

## Evaluation Metrics

- Classification Accuracy
- Cross-Entropy Loss
- Confusion Matrix
- Training Time
- Peak Memory Consumption

## Results

Key observations:

- PyTorch with GPU achieved the fastest training due to CUDA acceleration.
- Scratch implementation provided greater transparency into neural network training.
- Hardware significantly affected execution time but had minimal impact on final accuracy.
- All implementations achieved over 93% test accuracy on MNIST.

## Installation

Clone the repository

```bash
git clone https://github.com/arjun1151/CSOC-Week-2-ANNs.git
cd <repository-name>
```



## Frameworks Used

- Python
- NumPy
- PyTorch
- Matplotlib
- Scikit-learn


## Future Improvements
Future work could include experimenting with:

- Mini-batch Gradient Descent
- Adam Optimizer
- Learning Rate Scheduling
- Dropout Regularization
- Batch Normalization
