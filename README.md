Anime Face Generation using DCGAN

This project implements a Deep Convolutional Generative Adversarial Network (DCGAN) using TensorFlow and Keras to generate anime faces. The model is trained on Kaggle using a dataset of anime character images.

Project Overview

The project aims to generate high-quality anime face images by leveraging a DCGAN architecture. The model consists of:

Generator: A neural network that generates realistic anime faces from random noise.

Discriminator: A convolutional neural network that distinguishes between real and generated anime faces.

The two networks are trained together in an adversarial manner to improve the quality of generated images over time.

Dataset

The dataset contains a collection of anime face images, which are preprocessed and resized before training.

/data/anime-faces/
    ├── image1.jpg
    ├── image2.jpg
    ├── ...

Features

Implementation of DCGAN for realistic image generation.

Data preprocessing and augmentation.

Visualization of generated images at different epochs.

Training progress monitoring with loss curves.

Model saving and loading for future inference.

Training Process

The model is trained using TensorFlow and Keras on Kaggle with GPU acceleration.

The training alternates between optimizing the Generator and Discriminator.

Sample generated images are saved at regular intervals to monitor improvements.

Results

The generated anime faces improve over epochs, showing better-defined features and structure.

Evaluation metrics and loss curves help in tracking model performance.

How to Use

Clone this repository:

git clone https://github.com/Sahil489s/Anime-Face-Generation-DCGAN.git
cd Anime-Face-Generation-DCGAN

Install dependencies:

pip install tensorflow numpy matplotlib

Run the training script on Kaggle or a local GPU machine.

Model Saving & Loading

To save the trained generator:

generator.save("anime_generator.h5")

To load and generate new images:

from tensorflow.keras.models import load_model
generator = load_model("anime_generator.h5")
plot_training_progress(generator)

Acknowledgments

Kaggle for providing the dataset.

DCGAN architecture for enabling anime face generation.

