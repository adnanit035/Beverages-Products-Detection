# Beverages Products Detection using DETECTRON2 (September 2020)

This repository contains the code for the detection of beverages products using [Detectron2](https://github.com/facebookresearch/detectron2) project for a AI Bootcamp. The project was based on Computer Vision, focusing on object detection from scratch (data collection, annotation, model training, and deployment).

## Introduction
The project focuses on utilizing computer vision techniques, specifically object detection, to detect various beverage products such as Pepsi, Coke, and 7up using the Detectron2 framework. The project was divided into 4 main parts: data collection, data annotation, model training, and evaluating the model's performance.. The project was developed using Python and PyTorch. Initially focused on Pepsi products, the project was extended to include other categories like Coke and 7up products.

## Methodology and Process
The development process involves dataset preparation, model training, and testing.

### 1. Data Collection and Preparation
The dataset was collected from superstores shelves and refrigerators. Around 200 images were collected using a smartphone camera and split them into Train, Test and Validations sets by 80%, 10% and 10% respectively. Almost all of the images are real world and taken by myself. Only a few images (around 20) are taken from the internet but also they depict real world beverages on shelf. Then images were then annotated using the [VGG Image Annotator tool](https://www.robots.ox.ac.uk/~vgg/software/via/). Bounding boxes were drawn around the beverages products and the class labels were assigned. 

### 2. Model Training
The COCO-pretrained R50-FPN Mask R-CNN model was fine-tuned using Detectron2 on the annotated dataset.

### 3. Model Testing
The trained model was tested on both images and videos to evaluate its performance.

## Findings
The trained model was able to detect the beverage products with high accuracy. The model was able to detect the products in real-time and in images with high precision and recall. The mean Average Precision (mAP) for Pepsi, Coke, and 7up products was found to be 77%. The model was able to detect the products in different orientations, lighting conditions and even in videos with high accuracy.
