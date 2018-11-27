Neural networks (NN), also called Artificial Neural Networks (ANN) are a subset of learning algorithms within the machine learning field that are loosely based on the concept of biological neural networks.

Basically, an ANN comprises of the following components:

An input layer that receives data and pass it on
A hidden layer
An output layer
Weights between the layers
A deliberate activation function for every hidden layer.
 I am  creating  the feed-forward or perception neural networks. This type of ANN relays data directly from the front to the back.Training the feed-forward neurons often need back-propagation, which provides the network with corresponding set of inputs and outputs. When the input data is transmitted into the neuron, it is processed, and an output is generated.

To train our model , I made this sample training data , 

Training Data 1 - 0 0 1 Output - 0

Training Data 2 - 1 1 1 Output - 1

Training Data 3 - 1 0 1 Output - 1

Training Data 4  - 0 0 1 Output - 0

Training Data 5 - 0 1 1 Output - 0

Situation = 1 0 0 , output - ?

Since we can see that output is always the first no. of the array . So Expected output should be 1.

Even though I’ll not use a neural network library for this simple neural network example, I’ll import the numpy library to assist with the calculations.

The library comes with the following four important methods:

exp—for generating the natural exponential
array—for generating a matrix
dot—for multiplying matrices
random—for generating random numbers. Note that we’ll seed the random numbers to ensure their efficient distribution.
Applying the Sigmoid function
We’ll use the Sigmoid Function, which draws a characteristic “S”-shaped curve, as an activation function to the neural network.This function can map any value to a value from 0 to 1. It will assist us to normalize the weighted sum of the inputs.

we’ll create the derivative of the Sigmoid function to help in computing the essential adjustments to the weights.

The output of a Sigmoid function can be employed to generate its derivative. For example, if the output variable is “x”, then its derivative will be x * (1-x).

Training the model
This is the stage where we’ll teach the neural network to make an accurate prediction. Every input will have a weight—either positive or negative.

This implies that an input having a big number of positive weight or a big number of negative weight will influence the resulting output more.

Remember that we initially began by allocating every weight to a random number.

Here is the procedure for the training process we used in this neural network example problem:

We took the inputs from the training dataset, performed some adjustments based on their weights, and siphoned them via a method that computed the output of the ANN.
We computed the back-propagated error rate. In this case, it is the difference between neuron’s predicted output and the expected output of the training dataset.
We used the “.T” function for transposing the matrix from horizontal position to vertical position. Therefore, the numbers will be stored this way:

Ultimately, the weights of the neuron will be optimized for the provided training data. Consequently, if the neuron is made to think about a new situation, which is the same as the previous one, it could make an accurate prediction. This is how back-propagation takes place.



Code Output :-
![Screenshot](N_N.png)

So , we can see the output 0.99999853 which is close to 1 (Expected Value)

