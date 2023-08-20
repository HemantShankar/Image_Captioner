# Image_Captioner
- This is an implementation of an image caption generator which given an image generates a caption based on it. Image captioning is a challenging task where computer vision and natural language processing both play a part in generating captions. This technology can be used in many new fields like helping the visually impaired, medical image analysis, geospatial image analysis, etc.

- A trained Xception model is used to leverage the model's trained parameters to encode an image to a 2048 feature vector which is then fed into an LSTM to predict a caption based on the features extracted by Xception.

## Flow of the project
a. Cleaning the caption data

b. Extracting features from images using the Xception model

c. Merging the captions and images

d. Building LSTM model for training

e Predicting on test data

## Model Architecture
<img src="test_images/model_plot.png" width="800" height="400"></img>
## What is an encoder in such models?
The neural network that changes any input in its features representation i.e. vector of numbers is an encoder. For example, we want to use images to predict words. As images directly can't tell what the word should be, we want to use its feature to help us decide the next word. And thus the network of layers used to change image or any other type of input in its feature representation is known as encoders.

## What is a decoder?
The combination of layers/neural networks that takes feature representation provided by an encoder as its own input and predicts the next word, is known as a decoder
