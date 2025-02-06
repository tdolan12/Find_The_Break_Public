# Find The Break Public

## Overview

"Find The Break" is a computer vision project developed as part of the DATASCI 281 Computer Vision class at UC Berkeley. It aims to automate the detection of fractures in X-ray images using a combination of preprocessing, feature extraction, and classification techniques.

## Problem Addressed

Accurately diagnosing bone fractures from X-ray images is critical for effective treatment. However, human radiologists can sometimes overlook fractures due to fatigue or limitations in visual assessment. This project seeks to minimize human error by leveraging computer vision techniques to assist in fracture detection, improving diagnostic accuracy and efficiency.

## Features

- **Preprocessing Techniques**: Includes noise removal, contrast enhancement, and Canny Edge Detection to improve image quality.
- **Feature Extraction Methods**: Uses Gray-Level Co-Occurrence Matrix (GLCM), Local Binary Patterns (LBP), and features derived from a pre-trained ResNet-50 model.
- **Classification Models**: Evaluates multiple approaches, including linear models, Support Vector Machines (SVMs), Convolutional Neural Networks (CNNs), and other neural networks.
- **Model Optimization**: Conducts hyperparameter tuning and tests model generalization to ensure high accuracy and robustness.

## Authors

- **Thomas Dolan**
- **Charlie Glass**
- **Philippe Gagnon**
- **Meir T. Marmor**

### Instructor
- **Senthil Periaswamy**

## Directory Highlights

Although this is a public repository, the data and executable code are not available for direct access. Below are descriptions of the project structure and key files:

### **Final Report**
- **Documents/Proposal and Report/FindTheBreak_281 Final Report**: Contains the detailed final report, outlining the project methodology, experiments, and results.

### **Best Model**
- **Code/Best Hyperparameter Search Notebooks/parameter_tuning_no_preprocessing.ipynb**: Documents the search for the best-performing model, a Non-linear SVM trained on images with no preprocessing and 140 GLCM and LBP features.

### **Generalization Results**
- **Code/Best Hyperparameter Search Notebooks/FindTheBreak_281_Final_Project_Base_and_Best_Classifiers_Training_and_Testing.ipynb**: Evaluates model performance across different datasets to test generalization.

### **Bounding Box Experiment**
- **Code/bounding_box_experiment_pipeline.ipynb**: Explores bounding box detection for localizing fractures in X-ray images.

## Directory Structure

### **Code/**
Contains all executable code for the project, organized into subdirectories for specific tasks.

- **ResNet/CNN**: Scripts for building, training, and evaluating deep learning models.
- **EDA and Preprocessing**: Notebooks and scripts for Exploratory Data Analysis and preprocessing steps.
- **Best Hyperparameter Search Notebooks**: Documents the model optimization and generalization process.
- **Original Pipelines and Model Exploration**: Early-stage models, initial experiments, and data pipelines.

### **Slides/**
A collection of slide decks used for class presentations and project updates.

### **Documents/**
Supporting documentation, including:
- **Proposal and Reports**: PDFs of the project proposal and final reports.

### **Data/**
Stores X-ray images and related datasets.

- **Best Feature Extraction Train and Test CSV**: Contains CSV files with extracted features for training and testing.
- **Final Train and Test Image Folders**: Organized with an 80:20 split for training and testing datasets.

## License

This project is released under an open-source license. See [LICENSE](LICENSE) for more details.

## Contact

For any questions or discussions regarding this project, feel free to reach out to the authors.


