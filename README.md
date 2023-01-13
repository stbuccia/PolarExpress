# PolarExpress

Neural Network that learn mapping from polar to cartesian coordinates 

This is the project for [Machine Learning Course](https://www.unibo.it/en/teaching/course-unit-catalogue/course-unit/2022/412731) at [University of Bologna](https://www.unibo.it/en/homepage)

## Neural Network Specs

The defined Neural Network has:

*   2 input layer (separately for theta and rho) concatened in a single
*   2 hidden layer
*   1 output layer reshaped

And the number of neurons of every layer are:

*   Input layer: 
    - Numer of neurons: 1 (dimension of theta and rho)
*   First hidden layer: 
    - Number of neurons: 5 (arbitrary minimized)
    - Activation function: ReLU
*   Second hidden layer: 
    - Number of neurons: 5 (arbitrary minimized)
    - Activation function: ReLU
*   Output layer:  
    - Number of neurons:100 reshaped in 10x10 (dimension of output map)
    - Activation function: Softmax (In order to have a kind of probability over the output cells)

Other stuff:

*   Number of training samples: 4000
*   Number of test samples (for evaluationg accuracy): 200000
*   Batchsize: 128
*   Epochs: 150
*   Accuracy: about 95%
*   Number of params: 645
