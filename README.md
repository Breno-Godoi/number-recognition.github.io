Project Overview

This project showcases a fun and straightforward web application that allows you to draw a single-digit number, which is then recognized using simple machine learning techniques.

If you're eager to dive right into the code, here's what you'll find:

Google Colab Notebook for generating the Machine Learning Model.
HTML file containing the main application.
Let's get started! Below are the ingredients and steps required to build this demo.

Ingredients and Steps:

1. Training Data
For any Machine Learning model, high-quality data is essential. In this project, we're utilizing the MNIST dataset, which consists of handwritten digit images.

MNIST Dataset Example

This dataset includes 60,000 grayscale images of size 28 x 28 pixels, each with pixel values ranging from 0 to 255.

2. Training Environment
Google Colab provides a browser-based Python environment, allowing you to write and execute code seamlessly. It comes pre-loaded with essential Machine Learning libraries, making it a hassle-free platform for getting started with ML projects. Additionally, it offers free access to GPU/CPU resources.

3. Data Preprocessing
Before training our model, we need to preprocess the data from the MNIST dataset:

Normalize Inputs: Scale the pixel values from the range 0–255 to 0–1.
One-Hot Encode Outputs: Convert categorical labels to one-hot encoded vectors.
4. Machine Learning
We begin the Machine Learning process by building a simple Neural Network with one Hidden layer. This straightforward model achieves an accuracy of around 98%.

For those looking to go the extra mile, a Deep Learning Model is also presented. This model can achieve an impressive 99% accuracy.

5. Convert a Keras model to TensorFlow.js
With a trained model in hand, the next step is converting it for use with TensorFlow.js. This involves saving the model as an HDF5 file and then converting it to TensorFlow.js format.

6. HTML5 Canvas
The web application utilizes an HTML5 Canvas component, allowing users to draw their digit directly on the webpage. The drawing events are hooked to JavaScript functions, making it interactive and user-friendly.

7. Hooking Everything Up
The TensorFlow.js library is loaded onto the webpage, allowing us to load the trained model and make predictions based on user-drawn digits. The model is fed the scaled-down drawing data, and predictions are displayed on the webpage.


Check it here: https://breno-godoi.github.io/number-recognition.github.io/