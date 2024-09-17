Snake Species Identification - Model Creation and Testing

This project uses a Convolutional Neural Network (CNN) to classify snake species based on images. The model was developed using transfer learning to improve accuracy.
Project Objective

The goal of this project is to create a machine learning model that can accurately identify snake species from images. The model is integrated into a web app where users can upload images for prediction.
Model Overview

    Base Model: MobileNet (pretrained on ImageNet dataset)
    Fine-tuned: The model was fine-tuned on a custom dataset of snake species.
    Classes: The model can identify 7 different snake species, including:
        Cobra
        Common Krait
        Hump-Nosed Pit Viper
        Python
        Rat Snake
        Russell’s Viper
        Saw-Scaled Viper

Model Architecture

    Input: Image (224x224)
    Preprocessing: Images are preprocessed using MobileNet's standard preprocess_input function.
    Model: Transfer learning with MobileNet as the base model, followed by fully connected layers for classification.
    Output: Probability scores for each snake species.

Dependencies

    TensorFlow / Keras: For building and training the neural network.
    NumPy: For numerical operations.
    Pillow: For image processing.
    scikit-learn: For additional utilities like splitting the dataset.

Training

    Dataset: A custom dataset containing images of 7 snake species was used for training.
    Transfer Learning: The MobileNet model was used as the base, and additional layers were added to fine-tune it for snake species classification.
    Training Process:
        The model was trained for multiple epochs using Adam optimizer.
        Early stopping was applied to prevent overfitting.
