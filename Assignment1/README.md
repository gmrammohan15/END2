
Assignment 1 Questions

What is a neural network neuron? \ 
Neuron in neural network is a logical represention of entity in each layer of neural network which has set on input connections and output connections
from adjacent layers and holds temporary values.These connections are represented as weights and keeps changing based until we arrive at an optimal solution.
Each connection to a neuron is a mathematical function of weight and an non linear activation function.

What is the use of the learning rate? \ 
Learning rate is essentially a variable that helps us to tune the weights while doing gradient calculation or back propogation 
so that we reach the point of minimal loss without jumping or being too slow to reach that point
Lower the value, more time it takes to converge on minima and vice versa.Generally it is controlled for every training epochs.

How are weights initialized? \

Initialization of weights is one of the important steps in building neural networks.
Intiailizing weights to zero , will make neural networks linear which is not desired
Assiging low values result in vanishing gradient problems
Assigning random values may take longer time to reach convergence.

So generally statistical approach like normal or gaussian distribution is used to initialize weights.


What is "loss" in a neural network? \
Loss is the difference in expected/labelled output and what actually neural network spits or predicts for a given input.
Genrally mean square loss is applied for calculating gradients to adjust the weights in order to reduce the loss in next iteration.
Different types of loss functions are applied depending on use case.

What is the "chain rule" in gradient flow? \
Chain rules are applied while calculating gradients.Typical neural network comprises of more than one layer of neurons each internconnected
Partial derivates are applied for rate of change of loss wrt weights at each neuron.
So while backprogating the loss and calculating new weights since each layer is dependent on previous layer we need to accomodate that change as well while calculating the value for current one.
