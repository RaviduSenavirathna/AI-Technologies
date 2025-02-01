When data is input into the network, it passes through the network in the forward direction, from the input layer through the hidden layers to the output layer. This process is known as forward propagation. Here’s what happens during this phase:

**Linear Transformation:** 
- Each neuron in a layer receives inputs which are multiplied by the weights associated with the connections. These products are summed together and a bias is added to the sum. This can be represented mathematically as:

$$
z = w_{1}x_{1} + w_{2}x_{2} + \dots +w_{n}x_{n} + b
$$

where
`w` represents the weights
`x` represents the inputs
`b` is the bias

**Activation:** 
- The result of the linear transformation (denoted as z is then passed through an activation function. The activation function is crucial because it introduces non-linearity into the system, enabling the network to learn more complex patterns. 

- Popular activation functions include ReLU, sigmoid and tanh.