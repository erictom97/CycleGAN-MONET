# CycleGAN-MONET

# CycleGAN in PyTorch

This repository contains an implementation of CycleGAN using PyTorch, which allows you to convert images between two domains: MONET-style paintings and real photos. CycleGAN is a popular unsupervised image-to-image translation model that learns the mapping between two domains without paired training data. It has been widely used for various image translation tasks, such as style transfer, domain adaptation, and object transfiguration.

[IDEA](https://github.com/erictom97/CycleGAN-MONET/assets/40288848/95d88ebe-da55-42ea-9b3d-889b6ee029ac)




## Introduction

CycleGAN is based on the idea of cycle consistency, which enforces the translated image from one domain to be converted back to the original domain, while preserving its original content. This enables the model to learn meaningful mappings between the domains even without paired data. The architecture consists of two generator networks (for each domain) and two discriminator networks (for each domain). The generator networks aim to translate images from one domain to the other, while the discriminator networks distinguish between the generated and real images.

This implementation uses PyTorch, a popular deep learning framework, to build and train the CycleGAN model. It also provides utilities for handling the dataset, training the model, and testing the trained model on new images.



## Dataset

The dataset for CycleGAN consists of two sets of images: one for the MONET-style paintings and one for the real photos(Kaggle Dataset). The images in both sets should be aligned, meaning there should be corresponding images between the two domains. However, the datasets do not need to be paired. The model learns the mappings between the domains using unpaired images.


In the Code, `A` represents the MONET-style paintings and `B` represents the real photos.

## Results

The results of the CycleGAN model depend on various factors such as the dataset, training parameters, and model architecture. It is recommended to experiment with different configurations and hyperparameters to achieve the desired results.

Here are some example results obtained using this implementation:

![Samples](https://github.com/erictom97/CycleGAN-MONET/assets/40288848/d7760c58-87a3-4b3e-929a-388795e63500)
![LEX](https://github.com/erictom97/CycleGAN-MONET/assets/40288848/6f07c6cd-5a48-4af5-ab7f-892579179bbf)

## References:
Dataset:https://www.kaggle.com/competitions/gan-getting-started
Code: https://www.kaggle.com/code/songseungwon/cyclegan-tutorial-from-scratch-monet-to-photo
