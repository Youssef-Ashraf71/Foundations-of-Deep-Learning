## Lecture 2: Gradient Descent

# Least Average Euclidean Distance Model

## About

- This project is an implementation of the Least Average Euclidean Distance Model using the gradient descent algorithm to find the optimal point that minimizes the average Euclidean distance from a set of arbitrary points in Euclidean space.

## Methods

- [Using The definition of the derivative](link)

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

- step: the learning rate used in the gradient descent algorithm
- EPOCHS : the number of iterations used in the gradient descent algorithm
- DELTA: the convergence criterion used in the gradient descent algorithm
