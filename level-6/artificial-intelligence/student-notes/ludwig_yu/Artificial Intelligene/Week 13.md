Week 13

 # <section-title>Week 13</section-title>
 
* * *

### Learning Objectives
- Use the OpenAI gym library to implement a game simulation environment
- Develop a randoom game playing agent that can operate in an AI gym
- Use the keras library to build and train neural networks

* * *
##  What is OpenAI Gym
An OpenAI Gym is a way of providing standardised environments for reinforcement larning algorithms to operate in

Allows the developer to focus on agent instead of the simulation

Includes versioned, standard set of environment,s enabling easy comparsion.

### Avilable environments
Arcade Learning Environment 2013
Vizdoom 2016
OpenAI Gym 2016

**OpenAI Gym** aims to combine the best elements of theses previous benchmark collections, in a software package that is maximally convenient and accessible

### Keras and neural networks
#### What is a neural network
A set of processing units connected together into a 'netural network'

You feed some numbers in one end and other numbers come out of the other end

Training a neural network involves incrementally adjusting the settings of the processing units until they cause the correct outputs to come out inresponse to a set of inputs.

We put a set of inputs into the network, and compare the output with the desired output we want. Then we calculate the loss to see how "far" is the output away from what we want. Based on the loss, we adjust the setting of the network by rewiring the units.

DQN uses a neural network to learn the Q function, input is game state and output is the values of all actions.
##### Layers
Neural networks are made out of layers
There are different types of layers with different nodes in them which process the signal in different ways
##### Core Layers
Dense layer : just your regular densely-connected NN layer
Activation layer: Applies an activation function to an output
Embedding layer
Masking layer
Lambda layer
##### Convolutional Layers
Convolution layers (great for image processing)
Recurrent layers, LSTM,GRU(great for sequential data)
Attention layers (even better sequential data processing)
DQN uses some common layers plus some convolutional layers
##### Activation function
Activation functions dictate how certain types of nodes transfer the signal from input to output
##### Weights
Weights dictate the behavior of a layer.
Scaling the value of connections between nodes
Configuring the properties of more complex layers

Weights are the thing that we are adjusting over time with training
##### Loss function
how wrong is the neural network now
Loss functions dictate the error between the achieved and expected outputs
The loss is fed back into the network usiing back propagation

Distance functions are used as loss function, which calculate the difference between the desired and the actual output

##### Training 
Training involves feeding examples to the network in batches, calculating the loss and **feeding the loss back to the network weights**

Thus the network weights are iteratively changed to better model the disired or optimal input-output function. This processing new data then feeding back the difference continues until the network is good enough( the loss is low enough)
##### Custom loss functions
There are built-in loss functions but you might want to define your own

##### Complete picture for NN
1. Build model from layers
2. Initialise weights
3. Feed in batch of inputs
4. Calculate loss on outputs
5. Back propagate loss into the network
6. Back to 3.
#### What is keras
High level neural network API siting atop tensorflow
**The DQN example code we will look at uses keras**


### Convolutional Layer
The DQN network architecture uses convolutional layers
#### What is convolution
A filtering technique, often used for images but also other signals

Essentially, you calculate the new value for a pixel by adding together scaled values of the original pixel andites surrounding pixels
#### What does convolution do to images
You multiple each of the pixel values by the coefficient of the filter kernel
#### What is a convolutional layer
*learning a filter*
A neural network layer which applies trainable filters to image or other data.

Instead of heardcoding the filter parameters, we learn them
learning a filter

#### Convolution layer properties
a convolution layer applies mutiple filters to the image

A convolution layer has the following properties:
- **Filters**: how many filters we use(applied in paralled- stack layers to apply in series)
- **Size**: filter kernel size
- **Stride**: hop size (how many pixels move at a time)
#### Visualising convolutional layers
A great feature of convolutional layers is that we can visualise what they are doing to image data as it passes through the neural network