In this exercise we will train a network similar to the LeNet5 and use it for inference.
LeNet5 was the first successful CNN that was developed by Yann LeCunn in 1990 for classifying handwritten digits successfully. 
It can be deployed in applications such as reading handwritten ZIP and post codes, checks, and so on. 
I use dropout as a mitigation against overfitting.
Dropout is one of the most effective and most commonly used regularization techniques for neural networks, 
developed by Geof Hinton and his students at the University of Toronto. Hinton was inspired by the reason as to why
the bank constantly shuffles its 'cashiers' as a means to avoid fraud. He likened overfitting to a kind of fraud brought about
by a conspiracy between lower layers of a network and the upper layers. He believed that introducing some noise between layers
would reduce this conspiracy between layers; the upper layers would not know everything learned by lower layers and as such 
would be forced to work independently, somehow. He introduced this noise in the form of randomly "dropping out" (i.e. setting to zero)
some output features (information already learned) by the layer during training.

For example if the output of a given layer is a vector [0.3, 0.7, 1.5, 0.8, 1.3] for a given input sample during training; 
after applying dropout, this vector will have a few zero entries distributed at random, e.g. [0, 0.7, 1.5, 0, 1.3]. This is what get passed 
to the next upper layer. 
The "dropout rate" is the fraction of the features that are being zeroed-out and it's usually set between 0.2 and 0.5. 


I made use of knowledge from the following sources:

Deep Learning with Python by Francois Chollet
Deep Learning for Dummies by by John Paul Mueller and Luca Massaron



PS: I am doing data science and machine learning as a hobby but I wish to make it my life career!
cyprofusi@hotmail.com

