A neural network is a massively parallel distributed processor made up of simple processing units that has a natural propensity for storing experimental knowledge and making it available for use.
![[{9CE0487A-F7D1-47E1-A6F8-2932B6735B10}.png]]

Bias (b) has the effect of applying a transformation to weighted sum.
The bias is an external parameter of the neuron. It can be modeled by adding an extra input

Epoch: An Epoch represents one iteration over the entire dataset.

Batch: We cannot pass the entire dataset into ANN at once. So, we divide the dataset into number of batches

Iteration: If we have 1000 images as data and a batch size of 20 then an epoch should 1000/20 = 50 iteration.

Early Stopping: a technique commonly used to prevent overfitting and improve model generalization. it involves monitoring the performance of a model during training and stopping the training process before it reaches the point of overfitting

hyperparameters:
- number of layers
- number of neurons per layer
- type of activation function used in different layers
- error function
- learning algorithm
- learning rate
- weights and bias

Activitation functions:
- relu
- sigmoid
- softmax
- tanh