An activation function is applied to the weighted sum of inputs (before producing the final output of a neuron). It introduces non-linearity, enabling the model to learn and represent complex data patterns. Without it, even a deep neural network would behave like a simple linear regression model.
![[{5A1B8373-46F5-45F4-B8AD-53D918321EE1}.png | center|530]]

Activation functions decide whether a neuron should be activated based on the weighted sum of inputs and a bias term. They also make backpropagation possible by providing gradients for weight updates.

### Mathematical Example
Consider a neural network with:
- **Inputs**: $i_{1}$, $i_{2}$​
- **Hidden layer**: neurons $h_{1}$​ and $h_{2}$​
- **Output layer**: one neuron (output)
- **Weights**: $w_{1}, w_{2}, w_{3}, w_{4}, w_{5}, w_{6}$
- **Biases**: $b_{1}$​ for hidden layer, $b_{2}$​ for output layer

![[{8FC50A12-1BDF-4D3F-B3FC-40C19C575249}.png | center|503]]
Each circle represents a neuron (node) and a group of neurons forms a layer.

The hidden layer outputs are:
- $h_{1} = i_{1} . w_{1} + i_{2} . w_{3} + b_{1}$
- $h_{2} = i_{1} . w_{2} + i_{2} . w_{4} + b_{2}$​

The output before activation is:
- $output = h_{1} . w_{5} + h_{2} . w_{6} + bias$

Without activation, these are linear equations.

To introduce non-linearity, we apply a sigmoid activation:
$$
σ(x)= \frac{1}{1 + e^{-x}}
​$$
$final~output=σ(h_{1}.w_{5}+h_{2}.w_{6}+bias)$

This gives the final output of the network after applying the sigmoid activation function in output layers, introducing the desired non-linearity.

## Types of Activation Functions in Deep Learning

### Linear Activation Function
Linear Activation Function resembles straight line define by y=x. No matter how many layers the neural network contains if they all use linear activation functions the output is a linear combination of the input.
- The range of the output spans from (−∞ to +∞)(−∞ to +∞).
- Linear activation function is used at just one place i.e. output layer.
- Using linear activation across all layers makes the network's ability to learn complex patterns limited.

Linear activation functions are useful for specific tasks but must be combined with non-linear functions to enhance the neural network’s learning and predictive capabilities.


