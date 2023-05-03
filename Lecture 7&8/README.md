# Lecture 7 & 8: Automated Differentiation from Scratch || Computaional Graph

## Building An Autograd Engine from scratch

---

## About

In fact, building a computational graph using Python is one way to create an autograd engine from scratch. By representing the computation as a graph, it becomes easier to perform automatic differentiation and compute gradients with respect to the input variables.

This is because the graph structure captures the dependencies between the input variables and the intermediate computations, which is essential for computing the gradients using the chain rule.

There are several Python libraries that allow you to build computational graphs and perform automatic differentiation, including TensorFlow, PyTorch, and JAX. These libraries provide efficient implementations of autograd engines that can handle complex computations and run on both CPUs and GPUs.

This is a simple implementation of a computational graph using Python. The implementation can be used to perform simple arithmetic operations and apply elementary functions on them, while simultaneously keeping track of gradients through a backward propagation mechanism. The code can be used for both scalar and vector inputs.

---

## Backward Propagation

The implementation uses the chain rule for the backward propagation of gradients. The computational graph is composed of comp_node objects, which represent the nodes of the graph. Each node has a backward_prop function that updates its gradient using the gradients of its children. The backward_prop functions are defined according to the chain rule, which calculates the gradients of the output with respect to each node by multiplying the gradients of its children.
This from the pov of Forward pass 
---

## Supported Operations

- Addition (+)
- Subtraction (-)
- Multiplication (\*)
- Division (/)
- Power (^)
- Sine (sin)
- Cosine (cos)

---

## Test Case

```
from comp_node import comp_node

x = comp_node(val=2.0)
y = comp_node(val=3.0)

z = x * y
print(z.val) # prints 6.0

l = z + 1
print(l.val) # prints 7.0

l.backward_prop() # updates gradients

print(x.grad) # prints 3.0
print(y.grad) # prints 2.0
```

In this example, we create two comp_node objects, x and y, with initial values of 2.0 and 3.0, respectively. We then create a third comp_node object, z, which is the result of multiplying x and y. We create a fourth comp_node object, l, which is the result of adding z and 1. Finally, we call the backward_prop method on l to calculate the gradients with respect to x and y.

---

## Conclusion

This implementation provides a simple way to perform arithmetic operations on numbers and keep track of gradients through a computational graph. It can be used as a building block for more complex machine learning algorithms, such as neural networks.
