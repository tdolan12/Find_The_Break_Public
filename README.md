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

## Report
[![Find the Break Report](https://github.com/tdolan12/Find_The_Break_Public/blob/main/Report%20Image.png?raw=true)](https://github.com/tdolan12/Find_The_Break_Public/blob/main/FindTheBreak_281%20Final%20Report.pdf)

^^^ Click to Read Full Report ^^^

## Highlights

- Best Model: The highest performing model was a Non-linear SVM, achieving an AUC of 0.97, demonstrating superior accuracy in fracture detection.

- Feature Engineering: Implemented GLCM and LBP descriptors to capture texture features and ResNet-50 embeddings for deep learning-driven feature representation.

- Robust Preprocessing: Applied Gaussian filtering for noise removal, contrast enhancement, and Canny Edge Detection to highlight fracture structures.

- Generalization Results: The most generalizable model combined ResNet and LBP features, achieving 79% validation accuracy.

- Dimensionality Reduction: PCA analysis retained 99% variance, enhancing interpretability and efficiency.

- Bounding Box Detection: Conducted initial bounding box experiments for localizing fractures in X-ray images.

- Visualization & Analysis: TSNE and PCA visualizations provided insights into feature separability and model performance.

## Technical Notes

### **Data Collection & Preprocessing**
- The dataset, sourced from Kaggle, contains **9,363 X-ray images** evenly split between fractured and non-fractured cases.
- Images were resized to **224x224 pixels** for consistency.
- **Noise reduction** was applied using **Gaussian filtering** to remove salt-and-pepper noise.
- **Contrast enhancement** was performed to improve edge visibility.
- **Canny Edge Detection** was employed to highlight fracture structures.

### **Feature Extraction**
- **Gray-Level Co-Occurrence Matrix (GLCM)**: Captures texture relationships between pixel intensities, providing 140 extracted features.
- **Local Binary Patterns (LBP)**: Extracts texture information by comparing pixel intensities, generating 34 feature descriptors.
- **ResNet-50 Features**: A **pre-trained CNN model** extracts deep learning-based features for better representation.

### **Classification Models**
- Various classifiers were tested, including **Logistic Regression, Linear SVM, Non-linear SVM, and CNNs**.
- The **Non-linear SVM** model achieved the highest **AUC of 0.97**.
- A **ResNet-50 CNN** model was tested but did not outperform the SVM.

### **Model Evaluation & Optimization**
- **Principal Component Analysis (PCA)** reduced dimensionality while retaining **99% variance**.
- **TSNE visualization** illustrated non-linear separability in the dataset.
- **Hyperparameter tuning** was performed to optimize the best-performing models.

### **Bounding Box Experiment**
- Initial work on **bounding box detection** was conducted to explore localized fracture identification.
- Further refinements are required to enhance localization accuracy.


## License

This project is released under an open-source license. See [LICENSE](LICENSE) for more details.

## Contact

For any questions or discussions regarding this project, feel free to reach out to the authors.


