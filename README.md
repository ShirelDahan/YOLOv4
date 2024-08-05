# YOLOv4 Custom Object Detection
This repository contains the necessary configuration and setup to train a YOLOv4 model for custom object detection using Google Colab. The project leverages the powerful capabilities of YOLOv4 to detect objects specified by the user with high accuracy and speed.

## Project Overview
The goal of this project is to demonstrate how to train a YOLOv4 model on a custom dataset. This includes preparing the dataset, setting up the training environment in Google Colab, and providing instructions for training and evaluating the model.
This project involves enhancing object detection capabilities using the YOLOv4 . The objective is to leverage advanced neural network architectures for real-time object detection with improved accuracy.

## Features
- Custom dataset preparation guidelines.
- Training YOLOv4 on Google Colab with GPU support.
- Evaluation scripts to measure the model's performance.
- Example predictions and visualization.

### Prerequisites

- Google Colab account
- Basic knowledge of Python and neural networks
- Familiarity with object detection concepts

### Setup and Installation

1. **Clone the Repository:**
   git clone https://github.com/<your-username>/yolov4-custom-detection.git
   cd yolov4-custom-detection
   {This command is used to make a local copy of your GitHub repository.
   Replace <your-username> with your actual GitHub username,
   and if you named your repository something different,
   replace yolov4-custom-detection with your repository’s name.}
2. **Open Google Colab:**
   - Upload the notebook files from the colab_notebooks folder to your Google Colab.
   - Follow the instructions within each notebook.

  ### Dataset
  The dataset used for training includes various object classes. 
  The data was sourced from public datasets and was preprocessed to fit the input requirements of the YOLOv4 model, 
  including resizing images and converting annotations.

### Training the Model
   - Prepare your dataset according to the guidelines provided in the data_preparation.ipynb notebook.
   - Use the training.ipynb notebook to start the training process.
   - Monitor the training progress directly in Google Colab.

### Usage

# Example script to load and use the trained model
from yolov4 import YOLOv4
# Initialize detector
detector = YOLOv4()
# Load trained weights
detector.load_weights('<path-to-weights>')
# Perform detection
detections = detector.detect_objects('<path-to-image>')
# Print results
print(detections)

### Results
The model achieved promising results, with high precision and recall metrics. Visual outputs from the detections demonstrate the model's capability to accurately identify and localize objects in various conditions.
