# MNIST classifier and LMS Algorithm

## Character recognition using a trained MLP

The MNIST dataset of handwritten digits is one of the earliest and most commonly used datasets to benchmark machine learning classifiers.  Each datapoint contains 784 input features – the pixel values from a 28x28 image – and it belongs to one of 10 output classes – representing the numbers0–9.  We provide you with a pre-trained MLP using the MNIST dataset. The MLP has an input layer with 784-neurons, 2 hidden layers of 200 and 100 neurons, and a 10-neuron output layer.  The model assumes the ReLU activation for the hidden layers and the softmax function in the output layer.

-   Extract the weights and biases of the pre-trained network from mnist_network_params.hdf5. The file has 6 keys corresponding arraysW1,b1,W2,b2,W3,b3. Verify the dimension of each numpy array with the shape property.
-   The file mnist.testdata.hdf5 contains 10,000 images. xdata holds pixel intensities and ydata contains the corresponding class labels. Extract these.
-   Use numpy to create an MLP to classify each 784-dimensional image into the target 10-dimensional output.

## LMS algorithm for channel modeling/trackingConsider the the system