****Emotion Detection Using Deep Learning****

**Project Overview**
This project aims to develop a deep learning model capable of detecting human emotions from images. The model classifies images into seven emotion categories: Angry, Disgust, Fear, Happy, Neutral, Sad, and Surprise.

**Dataset**
The dataset used for training and validation is stored in the Emotion_dataset directory. It consists of:

Training data: Emotion_dataset/train/train
Validation data: Emotion_dataset/test/test
Each image is of size 48x48 pixels and has three color channels (RGB).

**Preprocessing**
Images are normalized by scaling pixel values to the range [0, 1]. Labels are one-hot encoded for categorical classification.

**Model Architecture**
The model is a Convolutional Neural Network (CNN) built using TensorFlow and Keras. It consists of:

Three convolutional layers with batch normalization, max pooling, and dropout.
Two dense layers with batch normalization and dropout.
A final dense layer with softmax activation for classification.
Training
The model is compiled with the Adam optimizer and categorical cross-entropy loss function. It is trained for 10 epochs with a batch size of 32.

**Evaluation**
The model's performance is evaluated using accuracy and loss on both the training and validation datasets.
