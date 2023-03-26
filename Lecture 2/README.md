## Lecture 2: Gradient Descent

# Least Average Euclidean Distance Model

## About

- This project is an implementation of the Least Average Euclidean Distance Model using the gradient descent algorithm to find the optimal point that minimizes the average Euclidean distance from a set of arbitrary points in Euclidean space.

## Methods

- [Using The definition of the derivative](https://github.com/Youssef-Ashraf71/Foundations-of-Deep-Learning/blob/main/Lecture%202/Least%20average%20euclidean%20distance%20Model.ipynb)

## Usage

To use this project, you will need to provide a set of arbitrary points in Euclidean space. You can define these points in a file called points.txt in the following format:

```
x1,y1,z1
x2,y2,z2
...
xn,yn,zn

```

- Once you have defined your points, you can run the Least average euclidean distance Model.ipynb script to find the optimal point that minimizes the average Euclidean distance:

```
python Least average euclidean distance Model.ipynb
```

- This will run the gradient descent algorithm and output the optimal point.

## Configuration

You can configure the gradient descent algorithm by adjusting the following parameters in the gradient_descent.py script:

- step:  determines the number of data points or samples that will be generated for the domain of the function being optimized.
- EPOCHS : the number of times the gradient descent algorithm will iterate over the training data.
- DELTA: represents the learning rate or step size for the gradient descent algorithm. The learning rate is a hyperparameter that determines the size of the step taken in the direction of the negative gradient while updating the model parameters (in this case x_p and y_p).
