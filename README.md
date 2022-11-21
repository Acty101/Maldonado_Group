# Analyzing cyclic voltammograms using a neural network with TensorFlow 2

*What is a cylic voltammogram? Here is an example below (IUPAC convention)<sup>1</sup>:*
<img src="https://cdn.shopify.com/s/files/1/0823/0287/files/cyclic-voltammogram-ferrocene-labelled_848x547.png?v=1644831341" alt="example_cylic_voltammogram" width="600"/> <sup>figure 1</sup>


A cyclic voltammogram (CV) is a graph of current against voltage and it is obtained by measuring output current of a varying potential difference across an electrode submerged in an electrolyte. It is proned to many variations depending on the element of the electrode used and the time that the electrode has been exposed to air (due to oxidation). <br>

*Here is an example of the variations (US convention)<sup>2</sup>*: <br>
<img src="https://raw.githubusercontent.com/Acty101/Maldonado_Group/main/figures/ja2c04991_0005.webp" alt="CV_variations" width="600"/> <sup>figure 2</sup>

The goal of this project is to build and train a neural network that can correctly classify these variations. I've used the Keras API from TensorFlow 2 to build a simple neural network with a total of 3 hidden layers. The hyperparameters were arbitarily set through trial and error on some testing datasets. My code works by reading in PNG files of CVs from each folder that corresponds to each category that the testing set needs to be classified into. This will be split into training/validation sets for the neural network. Using the same reading function, the experimental data (test set) is loaded in and calssified accordingly. The predictions are summarized in a bar chart and the results of all the predictions will then be used for further analysis into artifical photosynthesis by the Maldonado Group. Here is a link of their work: http://websites.umich.edu/~mgroup/

Note: Accurate training data for the neural network and my previously trained model are not available. Data is generated using MATLAB code (not mine) and will soon have upwards of 10,000 images split into hundreds of different categories.
<br>
<br>
<br>
<br>
<br>
<br>

<sup>*1: IUPAC convention: oxidative potential sweep is left to right, reductive potential sweep is right to left.<br>
2:* US convention: reductive potential sweep is left to right, oxidative potential sweep is right to left.</sup>
<br>
<br>
<sup>References:<br>
figure 1: https://www.ossila.com/pages/cyclic-voltammetry-applications <br>
Harry Robson, Chris Bracher <br>
figure 2: Photoinduced Charge Transfer from Quantum Dots Measured by Cyclic Voltammetry <br>
Micaela K. Homer, Ding-Yuan Kuo, Florence Y. Dou, and Brandi M. Cossairt <br>
Journal of the American Chemical Society 2022 144 (31), 14226-14234 <br>
  DOI: 10.1021/jacs.2c04991</sup>
