# Road Segmentation Using U-Net

This repository contains the code for a road segmentation model using the U-Net architecture. The model is trained on the DeepGlobe Road Extraction Dataset and can be used to extract road networks from satellite images.
Table of Contents

    Introduction
    Dataset
    Model Architecture
    Results

# Introduction

Road extraction from satellite imagery is an important task in the field of remote sensing and has various applications in urban planning, transportation management, and disaster response. This project aims to develop a deep learning model for accurate and efficient road segmentation.

The U-Net architecture, a widely used convolutional neural network for image segmentation, is employed in this project. The model is trained on the DeepGlobe Road Extraction Dataset, which contains satellite images and corresponding road masks.
Dataset

The DeepGlobe Road Extraction Dataset is used for training and evaluating the road segmentation model. The dataset consists of 6,226 satellite images and their corresponding road masks, with a resolution of 1024x1024 pixels.
# Model Architecture

The model used in this project is a modified version of the U-Net architecture. It consists of a contracting path (encoder) and an expansive path (decoder), with skip connections between the corresponding layers of the encoder and decoder.

The main components of the model are:

    Convolutional layers with ReLU activation
    Max pooling layers
    Batch normalization
    Dropout layers
    Upsampling layers
    Concatenation of feature maps from the encoder and decoder

The final layer of the model uses a sigmoid activation function to produce a binary road segmentation mask.

# Results
The U-Net model trained on the DeepGlobe Road Extraction Dataset achieves a Jaccard coefficient (Intersection over Union) of 31.6 on the validation set.
