# Deep Learning
![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/4c69f115-4195-4a30-944b-0c853d38a352)

- A neural network (also called an artificial neural network) is an adaptive system that learns by using interconnected nodes or neurons in a layered structure that resembles a human brain. A neural network can learn from data—so it can be trained to recognize patterns, classify data, and forecast future events.
- It consists of an input layer, one or more hidden layers, and an output layer. In each layer there are several nodes, or neurons, with each layer using the output of the previous layer as its input, so neurons interconnect the different layers. Each neuron typically has weights that are adjusted during the learning process, and as the weight decreases or increases, it changes the strength of the signal of that neuron.

## Logistic Regression as a Neural Network
- how Logistic regression is implemented for a binary classification, here a Cat vs. Non-Cat classification, which would take an image as an input and output a label to propagation whether this image is a cat (label 1) or not (label 0).

- An image is store in the computer in three separate matrices corresponding to the Red, Green, and Blue color channels of the image. The three matrices have the same size as the image, for example, the resolution of the cat image is 64 pixels x 64 pixels, the three matrices (RGB) are 64 by 64 each. To create a feature vector, x, the pixel intensity values will be “unroll” or “reshape” for each color. The dimension of the input feature vector x is n_x=64\times64\times3=12288.

- Logistic Regression Cost Function
In Logistic regression, we want to train the parameters w and b, we need to define a cost function.

<img width="343" alt="image" src="https://github.com/ankitrajput77/Data.Science/assets/113281225/e3a41241-642a-4976-b7e3-928a931c641e">

The loss function measures the discrepancy between the prediction (𝑦̂(𝑖)) and the desired output (𝑦(𝑖)). In other words, the loss function computes the error for a single training example.
![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/062ff24b-5a46-4a3c-8a15-a981ce3fad23)

- The cost function is the average of the loss function of the entire training set. We are going to find the parameters 𝑤 𝑎𝑛𝑑 𝑏 that minimize the overall cost function.
![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/756f6518-c633-4b16-86e0-f131da7cbfbc)
- The loss function measures how well the model is doing on the single training example, whereas the cost function measures how well the parameters w and b are doing on the entire training set.
- 
