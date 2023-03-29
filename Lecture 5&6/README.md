## Lecture 5 & 6 : Pytorch & Supervised Learning

# Building a Classifier for the Two-Moon Dataset

## Introduction

In this project, we will build a classifier capable of categorizing unseen examples as either belonging to one of the moons in the two-moon dataset. This dataset is commonly used in machine learning to demonstrate the effectiveness of classification algorithms.

## Dataset

The two-moon dataset is a synthetic dataset that consists of two interleaving half circles. It is often used to test the effectiveness of binary classification algorithms. The dataset is generated using the make_moons() function from the scikit-learn library.

## Approach

We will use the cross-entropy loss function to optimize the weights of the network. The neural network will be implemented using the PyTorch framework.

## Dependencies

To run this project, you will need:

- Python 3.6 or higher
- PyTorch 1.9.0 or higher
- NumPy
- Matplotlib
  You can install all of these dependencies using the following command:

```
pip install torch numpy matplotlib
```
