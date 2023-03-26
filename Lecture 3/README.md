# Least Average Euclidean Distance Model

## About

- This project is an implementation of the Least Average Euclidean Distance Model using the gradient descent algorithm to find the optimal point that minimizes the average Euclidean distance from a set of arbitrary points in Euclidean space.

## Methods

- [Using Closed Form evaluated by backward Propagation](link)

## Concept

Backpropagation is a widely used algorithm for calculating the gradients in neural networks. The algorithm works by propagating the error gradient backward through the network from the output layer to the input layer, while updating the weights in each layer to minimize the error.

Here are the steps for using backpropagation to calculate the gradient:

- Forward Pass: Compute the output of the neural network for a given input, using the current values of the weights and biases in each layer. This involves calculating the weighted sum of the inputs and applying the activation function for each neuron in each layer.

- Error Calculation: Calculate the error between the predicted output and the desired output for the given input. This is typically done using a loss function such as mean squared error or cross-entropy.

- Backward Pass: Propagate the error gradient backward through the network from the output layer to the input layer. This is done by calculating the gradient of the loss function with respect to the output of each neuron in each layer.

- Weight Update: Update the weights and biases in each layer using the calculated gradients and a learning rate. This involves subtracting a small fraction of the gradient from each weight and bias in the network.

- Repeat: Repeat steps 1-4 for a number of iterations or until the error is minimized to an acceptable level.

Overall, backpropagation is an efficient algorithm for computing gradients in neural networks and is widely used in various machine learning applications.

## Configuration

You can configure the gradient descent algorithm by adjusting the following parameters in the gradient_descent.py script:

- step: determines the number of data points or samples that will be generated for the domain of the function being optimized.
- EPOCHS : the number of times the gradient descent algorithm will iterate over the training data.
- DELTA: represents the learning rate or step size for the gradient descent algorithm. The learning rate is a hyperparameter that determines the size of the step taken in the direction of the negative gradient while updating the model parameters (in this case x_p and y_p).
