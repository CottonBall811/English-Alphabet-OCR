# CottonBall-English-Alphabet-OCR
This is a simple program to build a model for recognizing English letters. By neural network, this program can be run to build a model and improve it and reaches a accuracy about 99 percent.
## How it work
Neural network is the most popular machine learning model in Artificial Intelligence industry, which is stimulating human's neural network. By adjusting the values of weight and bias, which are neural network parameters, the model can be promoted in the period of training.  
Several neurons make up a layers and several layers make up the neural network. There are three fundamental layers, an input layer, several hidden layers and an output layer. The data is transmitted to the inner layer. After calculating and passing through the inner layers, the result is outputed by the output layer.  
The structure of the neural network is shown in the following figure.  
![neural network](https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Neural_network_example.svg/1200px-Neural_network_example.svg.png)
In this program, there are two *fullyconnect layers* and a sigmoid function after each fullyconnect layers. The sigmoid function can convert the number into a number which between 0 and 1. It can also be seen as a probability. And it is easy to get its derivation. However, the change of sigmoid is little which leads to the step length to be little. Hence, a *cross entropy function* is used in the final part of the hidden layers to counteract the derivation of sigmoid function. By testing several times, the model with two fullyconect layers is better than one layer. Although the model with three fullyconnect layers is also better than two layers, it costs much longer time for each test. That is why there are two fullyconnect layers in this program.  
For the *&learning rate*, after more than 100 tests, 1250 is selected to be the learning rate.
## Source
Training data can be accessed from <http://arxiv.org/abs/1702.05373> and <http://archive.ics.uci.edu/ml>.  
The preprocess.py is the module to convert the training data into numpy arrays.  
The train.py is the training module.  
The value of weight and bias of different accuracy have been put up in the files.  
## Further implementation
The OCR application is looking forward to be implemented.  
***Your Suggestions and comments are welcome!***
