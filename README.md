# Analyzing cyclic voltammograms using a neural network with TensorFlow 2 (Maldonado Lab)

*What is a cylic voltammogram? Here is an example below:*
![example_cylic_voltammogram](https://cdn.shopify.com/s/files/1/0823/0287/files/cyclic-voltammogram-ferrocene-labelled_848x547.png?v=1644831341)

A cyclic voltammogram is a graph of current against voltage and it is obtained by measuring output current by varying potential difference across an electrode submerged in an electrolyte. It is proned to many variations depending on the element of the electrode used and the time said electrode has been exposed to air. 

The goal of this project is to build and train a neural network that can correctly classify these variations. I've used the Keras API from TensorFlow 2 to build a simple neural network with a total of 3 hidden layers. The hyperparameters were arbitarily set through trial and error on some testing datasets. My code works by reading in many PNG files of the same dimensions from each folder that corresponds to each category that the testing set needs to be classified into. The results will be used for further analysis by the Maldonado Lab.

Note: Accurate training data for the neural network and my previously trained model are not available. Data is generated using MATLAB code (not mine) and will soon have upwards of 10,000 images split into hundreds of different categories.
