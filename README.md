# Fashion-Generator-B-W
This repository contains GAN network to generate black and white fashion images

# Introduction

The FashionGAN project is a creative exploration into generative adversarial networks (GANs) specifically tailored for generating fashion images. GANs, a powerful subset of machine learning models, consist of two neural networks—the generator and the discriminator—that are trained together to produce realistic images from random noise. The generator learns to create images that mimic real fashion designs, while the discriminator tries to distinguish between the generator's fake images and actual fashion images. Over time, this adversarial process results in the generator producing increasingly convincing fashion images that are almost indistinguishable from real-life examples.

This project utilizes a comprehensive dataset of fashion images to train the GAN model. By feeding the generator network with random noise vectors, it learns to generate a diverse range of fashion items, from casual wear to formal attire, capturing various styles, patterns, and colors. This enables us to explore and visualize new fashion designs that do not exist in the current market, providing insights into potential future trends. The trained generator model can be used to inspire designers or even to automate the initial design process, pushing the boundaries of creativity in fashion.

Through this README, you will find a detailed guide on how to replicate the results, the underlying theory behind GANs, and instructions on how to use the trained model for your own fashion image generation needs.

# Dataset Overview

The dataset used for this project is the FashionMNIST dataset from TensorFlow. FashionMNIST is a popular dataset consisting of grayscale images of fashion items. It contains 60,000 training images and 10,000 testing images, each of size 28x28 pixels, depicting various clothing items such as shirts, trousers, shoes, and bags. The images are labeled into one of ten classes, representing different types of fashion items. This dataset is strictly in black and white, providing a challenging task for generating realistic images through a Generative Adversarial Network (GAN). The simplicity of the images, coupled with the nuanced differences between classes, makes FashionMNIST a compelling choice for exploring generative models in computer vision.

To prepare the dataset for training, standerd tensorflow dataset pipeline was set. First, the images were loaded and normalized using a custom function to scale the pixel values to a range between 0 and 1, which is essential for stable GAN training. The dataset was then cached to improve data retrieval speed, shuffled to ensure randomness in the training process, and batched into groups of 128 images to efficiently manage memory usage and optimize training performance. Finally, prefetching was used to overlap data preprocessing with model execution, reducing the likelihood of bottlenecks and improving the overall efficiency of the training process.

# Model Architecture




