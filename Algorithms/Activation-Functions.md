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

### Non-Linear Activation Functions
**Sigmoid Function**
Sigmoid activation function is characterized by 'S' shape. It is mathematically defined as
$$ A = \frac{1}{1+e^{-x}}$$
This formula ensures a smooth and continuous output that is essential for gradient-based optimization methods.

- It allows neural networks to handle and model complex patterns that linear equations cannot.
- The output ranges between 0 and 1, hence useful for binary classification.
- The function exhibits a steep gradient when x values are between -2 and 2. This sensitivity means that small changes in input x can cause significant changes in output y which is critical during the training process.


**Tanh Activation Function**
Tanh function (hyperbolic tangent function) is a shifted version of the sigmoid, allowing it to stretch across the y-axis. It is defined as:
$$
f(x)=tanh⁡(x)=\frac{2}{1+e^{-2x}}-1
$$
Alternatively, it can be expressed using the sigmoid function:
$$
tanh⁡(x)=2×sigmoid(2x)−1
$$
- Value Range: Outputs values from -1 to +1.
- Non-linear: Enables modeling of complex data patterns.
- Use in Hidden Layers: Commonly used in hidden layers due to its zero-centered output, facilitating easier learning for subsequent layers.


**ReLU (Rectified Linear Unit) Function**
ReLU activation is defined by $A(x)=max⁡(0,x)$, this means that if the input x is positive, ReLU returns x, if the input is negative, it returns 0.

- Value Range: (0,∞), meaning the function only outputs non-negative values.
- Nature: It is a non-linear activation function, allowing neural networks to learn complex patterns and making backpropagation more efficient.
- Advantage over other Activation: ReLU is less computationally expensive than tanh and sigmoid because it involves simpler mathematical operations. At a time only a few neurons are activated making the network sparse making it efficient and easy for computation.


**Leaky ReLU**
$$
f(x) = \begin{cases} x, & x > 0 \\ \alpha x, & x \le 0 \end{cases}​
$$
- Leaky ReLU is similar to ReLU but allows a small negative slope (αα, e.g., 0.01) instead of zero.
- Solves the “dying ReLU” problem, where neurons get stuck with zero outputs.
- Range: (−∞,∞)(−∞,∞).
- Preferred in some cases for better gradient flow.


**SoftPlus Function**
Softplus function is defined mathematically as: 
$$
A(x)=log⁡(1+e^x)
$$
This equation ensures that the output is always positive and differentiable at all points which is an advantage over the traditional ReLU function.

- Nature: The Softplus function is non-linear.
- Range: The function outputs values in the range (0,∞)(0,∞), similar to ReLU, but without the hard zero threshold that ReLU has.
- Smoothness: Softplus is a smooth, continuous function, meaning it avoids the sharp discontinuities of ReLU which can sometimes lead to problems during optimization.

### Exponential Linear Units
**ELU (Exponential Linear Unit) Function**
ELU (Exponential Linear Unit) is a non-linear activation function designed to improve learning speed and reduce the vanishing gradient problem. It behaves like ReLU for positive inputs but allows smooth negative values instead of zero, which helps the network learn more balanced representations.
$$
f(x) = \begin{cases} x, & x > 0 \\ \alpha(e^x - 1), & x \le 0 \end{cases}​
$$
- Value Range: (−α,∞)(-\alpha, \infty)(−α,∞)
- Non-linear: Helps neural networks model complex patterns
- Negative Outputs: Unlike ReLU, ELU allows negative values, making outputs closer to zero mean
- Smooth Curve: Continuous and differentiable, helping stable training


**SELU (Scaled Exponential Linear Unit) Function**
SELU is a scaled version of ELU designed for self-normalizing neural networks. It automatically keeps neuron outputs close to zero mean and unit variance, which stabilizes training. It is defined as:
$$
f(x) = \lambda \begin{cases} x, & x > 0 \\ \alpha(e^x - 1), & x \le 0 \end{cases}
$$
where λ ≈ 1.05 (scaling factor) and α ≈ 1.67

- Value Range: (−λα,∞)(−λα,∞)
- Self-Normalizing: Keeps activations stable across layers.
- Improves Gradient Flow: Helps prevent exploding or vanishing gradients.
- Works Best With: Deep fully connected networks using proper initialization and dropout variants.
- Reduces Need for Batch Normalization in some architectures.

### Output Layer Activation Functions
**Sigmoid Activation Function**
Sigmoid function produces an S-shaped curve and maps input values into a probability-like range between 0 and 1 and is used to find the final output of the neural network for binary classification problems. It is defined as:
$$
σ(x)= \frac{1}{1+e^{-x}}​
$$
- Value Range: (0,1)(0,1)(0,1)
- Smooth and Differentiable: Useful for gradient-based optimization.
- Best for: Binary classification output layers.
- Interpretable Output: Can be treated as probability.
- Limitation: Suffers from vanishing gradient for very large or very small inputs.


**Softmax Function**
Softmax function is designed to handle multi-class classification problems. It transforms raw output scores from a neural network into probabilities. It works by squashing the output values of each class into the range of 0 to 1 while ensuring that the sum of all probabilities equals 1.

- Softmax is a non-linear activation function.
- The Softmax function ensures that each class is assigned a probability, helping to identify which class the input belongs to.
