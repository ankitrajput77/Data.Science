# Deep Learning
![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/4c69f115-4195-4a30-944b-0c853d38a352)

- A neural network (also called an artificial neural network) is an adaptive system that learns by using interconnected nodes or neurons in a layered structure that resembles a human brain. A neural network can learn from data—so it can be trained to recognize patterns, classify data, and forecast future events.
- It consists of an input layer, one or more hidden layers, and an output layer. In each layer there are several nodes, or neurons, with each layer using the output of the previous layer as its input, so neurons interconnect the different layers. Each neuron typically has weights that are adjusted during the learning process, and as the weight decreases or increases, it changes the strength of the signal of that neuron.

## why we use activation functions
1. Non-linearity: Activation functions introduce non-linearity into the network. Without non-linearity, the entire network, no matter how deep, would behave as a linear model, making it limited in its ability to model complex relationships in data. Non-linear activation functions like ReLU (Rectified Linear Unit), Sigmoid, and Tanh allow neural networks to approximate and learn complex, non-linear mappings between inputs and outputs.

2. Gradient Flow: Activation functions help in the backpropagation algorithm, which is used to train neural networks. Non-linear activation functions ensure that gradients can flow backward through the network, which is necessary for updating the model's weights and minimizing the loss function.

3. Normalization: Activation functions can help in normalizing the outputs of neurons. For example, Sigmoid and Tanh functions squish their inputs into a range between 0 and 1 or -1 and 1, respectively. This can help control the scale of the outputs and make optimization more stable.

4. Sparsity: Some activation functions, like ReLU, can induce sparsity in the network. ReLU units produce zero output for all negative inputs, which can lead to sparse representations, helping in feature selection and reducing overfitting.

5. Vanishing and Exploding Gradients: Some activation functions can mitigate the vanishing and exploding gradient problems that arise during training in deep networks. For instance, ReLU helps avoid the vanishing gradient problem by allowing gradients to flow for positive inputs, while still imposing an upper limit, preventing exploding gradients.

6. Squashing Outputs: Certain activation functions like Sigmoid and Tanh squish the outputs within a finite range, which can be advantageous when the network needs to produce probabilities or values within a specific range.


