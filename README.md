# Vision Transformer for Cats vs Dogs Classification

## Project Overview

This project demonstrates binary image classification using a Vision Transformer (ViT) model to classify images of cats and dogs. The model is trained and tested on the popular Cats vs Dogs dataset from Kaggle.

ViT is particularly well-suited for this task as it leverages the Transformer architecture to capture complex relationships between image pixels.

## Dataset

The dataset used in this project is the **https://www.kaggle.com/competitions/dogs-vs-cats/data** Dataset from Kaggle. It contains 25,000 labeled images (12,500 cats and 12,500 dogs).

## Project Structure

- `vit-cats-vs-dogs-pytorch.ipynb`: The Jupyter Notebook containing the code for training and testing the model.
- `README.md`: This file, which provides an overview and instructions for the project.

## Model Architecture

First I write code of ViT transformer model from paper with 500 images for training and 50 images for testing that give me very bad result less than 50% accuracy. Then I try pretrain vit model give me outstanding result. After that I increase the amount of train data I take 20% of main train data and train my model that give almost 100% accuracy.
Here is the Vit transformer image and some parameter I choose.

![ViT](https://github.com/user-attachments/assets/b1034739-25fa-4b10-ac49-11b2667318e7)

- Backbone: Pretrained ViT model from PyTorch's torchvision library.
- Optimizer: Adam optimizer.
- Loss Function: Cross-entropy loss.
- Training Epochs: 10.

## Why Vision Transformer?

Vision Transformers have proven effective in image classification tasks as they:

- Use self-attention mechanisms to capture global relationships across image patches.
- Often outperform convolutional neural networks (CNNs) on large datasets.
- Provide a flexible framework for fine-tuning on specific tasks.


