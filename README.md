# Melanoma Skin Cancer Detection

## Problem Statement

In the skin biopsy, the dermatologist takes some part of the skin lesion and examines it under the microscope. The current process takes almost a week or more, starting from getting a dermatologist appointment to getting a biopsy report.
The aims to shorten the current gap to just a couple of days by providing the predictive model.
The approach uses Convolutional Neural Network (CNN) to classify nine types of skin cancer from outlier lesions images. This reduction of a gap has the opportunity to impact millions of people positively.

## Dataset

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images.

## CNN Architecture Design

To categorize skin cancer based on skin lesion images, I developed a custom CNN model to enhance accuracy and performance in the classification task.

- Rescaling Layer: This layer adjusts the input from the [0, 255] range to the [0, 1] range.
- Convolutional Layer: These layers apply convolution operations to the input, condensing the information within a receptive field into a single value. This process reduces image size while consolidating information.
- Pooling Layer: Used to decrease feature map dimensions, the pooling layer summarizes features within specific regions of the convolution layer's output.
- Dropout Layer: Introducing randomness during training by setting input units to 0 at each step helps prevent overfitting.
- Flatten Layer: This layer transforms data into a 1-dimensional array, enabling input to the subsequent layer. It's utilized after convolutional layers to create a lengthy feature vector connected to the final fully-connected layer, which drives classification.
- Dense Layer: Neurons in this layer are densely connected, meaning each neuron receives input from all neurons in the preceding layer.
- Activation Function (ReLU): The rectified linear activation function outputs input directly if positive; otherwise, it outputs zero. It tackles the vanishing gradient problem, facilitating faster learning and improved performance.
- Activation Function (Softmax): Deployed in the output layer of models predicting multinomial probability distributions, the softmax function ensures output probabilities range from 0 to 1, with the sum equating to one. This provides interpretable output probabilities.

## Contact

Created by Harikesh Madhava Kumar(HariMK01) - feel free to contact me!
