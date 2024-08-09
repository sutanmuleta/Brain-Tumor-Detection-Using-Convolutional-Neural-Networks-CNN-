# Brain-Tumor-Detection-Using-Convolutional-Neural-Networks-CNN-


## Overview

This repository contains a deep learning model for the automated detection and classification of brain tumors from MRI scans. The model is built on the **ResNet50 architecture**, utilizing convolutional neural networks (CNNs) to enhance diagnostic accuracy and efficiency.

## Problem Statement

Diagnosing brain tumors accurately is crucial but challenging, especially when relying on manual methods by radiologists. These methods can be time-consuming and prone to errors. This project aims to automate the classification process to improve both speed and accuracy, ultimately benefiting patient care.

## Key Features

- **ResNet50 architecture**: A proven model for image classification, tailored here for brain tumor detection.
- **Data augmentation**: Techniques such as rotation and flipping are used to improve the model’s robustness.
- **Model explainability**: The model includes features that help clinicians understand its decision-making process.
- **Ethical considerations**: Patient data privacy is ensured through compliance with GDPR and HIPAA, and efforts were made to minimize bias in the model.

## Dataset

The model was trained on 3,762 MRI images, split evenly between tumor and non-tumor cases. Images were resized to 128x128 pixels and preprocessed to standardize quality.

## Model Development

### Architecture

- **Base model**: ResNet50
- **Layers**: Convolutional, pooling, and dense layers
- **Output layer**: Softmax activation for binary classification

### Training and Fine-Tuning

- **Data split**: 70% training, 15% validation, 15% test
- **Optimizer**: Adam
- **Loss function**: Binary cross-entropy
- **Hyperparameters**:
  - **Learning rate**: Dynamically adjusted
  - **Epochs**: 50
  - **Batch size**: 32

## Evaluation

The model was evaluated using accuracy, precision, recall, and F1-score, showing strong performance in distinguishing between tumor and non-tumor MRI scans.

## Ethical Considerations

- **Data privacy**: Patient data was anonymized to comply with GDPR and HIPAA.
- **Bias mitigation**: Efforts were made to ensure the model performs fairly across different patient groups.

## Future Work

- **Dataset expansion**: Plans to include more diverse data to improve model robustness.
- **Hyperparameter tuning**: Further optimization of model parameters.
- **Clinical testing**: Developing user interfaces and testing the model in real-world settings.
- **Explainability**: Continued work to enhance model transparency.

## Conclusion

This project demonstrates the potential of AI in medical diagnostics, particularly in the accurate and efficient classification of brain tumors. The model emphasizes ethical practices and explainability, essential for its adoption in healthcare.
