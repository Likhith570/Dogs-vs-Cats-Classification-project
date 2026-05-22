# Dogs-vs-Cats-Classification-project
This project demonstrates a simple Convolutional Neural Network (CNN) built with TensorFlow and Keras to classify images as either "Cat" or "Dog".

Project Overview
The notebook implements a binary image classifier using a Sequential CNN architecture, designed to process images resized to 64x64 pixels.

Model Architecture
The CNN architecture consists of the following layers:

Conv2D (32 filters, 3x3 kernel): Extracts spatial features from input images.

MaxPooling2D (2x2 pool size): Reduces the spatial dimensions of the feature maps.

Conv2D (32 filters, 3x3 kernel): Adds another layer of feature extraction.

MaxPooling2D (2x2 pool size): Further reduces spatial dimensions.

Flatten: Converts the 3D feature maps into a 1D vector.

Dense (128 neurons): Fully connected hidden layer for classification.

Dense (1 neuron, sigmoid activation): Final output layer for binary classification (Cat vs. Dog).

Data Preprocessing
The model utilizes ImageDataGenerator for data loading and preprocessing:

Rescaling: Normalizes pixel values to the range [0, 1].

Augmentation (Training set only): Includes shear_range, zoom_range, and horizontal_flip to improve model generalization.

Input Scaling: Images are standardized to a target size of 64x64 pixels.

Usage Notes
Model Loading: The notebook includes code to load a pre-existing model (dogcat_model_bak.h5) for further training or evaluation.
