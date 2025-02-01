Forward propagation in neural networks is the process where input data flows through each layer of the model to generate an output. It’s the step-by-step computation that transforms raw inputs into predictions using weights, biases and activation functions. This operation forms the backbone of how neural networks learn patterns and make decisions.
![[{894CA55F-53AC-4C5E-A876-7D9136F96BA0}.png | center | 485]]

- It computes intermediate values layer by layer, starting from the input layer and ending at the output layer.
- Each neuron applies weighted sums and activation functions to extract features.
- It is used during both training and inference, but without weight updates.
- The accuracy of predictions heavily depends on how well forward propagation captures patterns from the input data.

#### The process of Forward Propagation
**Input Layer:** 
The network begins by receiving raw data through the input layer. Each feature in the dataset corresponds to a neuron in this layer, allowing the model to read all required information. Before entering the network, the data is often normalized or standardized to ensure faster training and better stability.

**Hidden Layers:** 
The processed input then passes through one or more hidden layers, where most of the computation happens. Every neuron in a hidden layer performs a weighted calculation on its inputs and then applies an activation function to introduce non-linearity. The computation inside each neuron follows:

$$
Z=W×X+b
$$
where:
`W` represents the weights
`X` is the input vector
`b` is the bias term

After this, an activation function such as ReLU or sigmoid is applied to produce the neuron’s output, which is then passed forward.

**Output Layer:** 
The final layer generates the model’s prediction. The choice of activation function depends on the task:

Softmax → multi-class classification
Sigmoid → binary classification
Linear → regression
This layer converts the processed information into a meaningful output.

**Prediction:** 
Based on the current weights and biases, the network produces its final output. The prediction is then compared with the true value using a loss function which calculates the error and sends it to backpropagation for learning.