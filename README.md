# CIFAR-10 CNN Architecture & Optimization Experiments

## Overview
This repository contains practical experiments and a comprehensive analysis of Convolutional Neural Network (CNN) models for image classification. The project aims to study and evaluate the impact of various data preprocessing techniques and architecture tuning to achieve the best possible accuracy and reduce overfitting.

## Dataset
The models were built and trained on the popular **CIFAR-10** dataset, which contains color images categorized into 10 classes (such as airplanes, automobiles, birds, cats, etc.). The data in this project is split into:
* **Training Data:** 40,000 images.
* **Validation Data:** 10,000 images.
* **Testing Data:** 10,000 images.

## Key Experiments
This project is divided into several main experiments and comparisons supported by plotted curves:

### 1. Data Preprocessing Comparison
* Testing the baseline model without preprocessing (pixel range 0-255).
* Normalization using Min-Max scaling ([0,1]).
* Data standardization using calculated mean and standard deviation.

### 2. Impact of Data Augmentation
* Comparing model performance with and without using the `ImageDataGenerator` tool.
* Applying operations like rotation, width/height shifts, horizontal flips, and zoom to improve model generalization and reduce the overfit gap between training and validation accuracy.

### 3. CNN Architecture Tuning
* **Filter Count Comparison:** Comparing network performance using different filter sizes (Small, Medium, and Large configurations) to test model capacity.
* **Network Depth Comparison:** Building and training three models with varying depths (Shallow, Medium Depth, and Deep). 
* Utilizing `GlobalAveragePooling2D` and `MaxPooling2D` layers to optimally control the network's parameters.

## Technologies Used
* **Python 3**.
* **TensorFlow & Keras** for building and training deep learning models.
* **NumPy** for matrix and array processing.
* **Matplotlib & Seaborn** for plotting performance curves (Loss & Accuracy) and confusion matrices.
* **Scikit-learn** for performance evaluation metrics (Classification Report).

## How to Run
1. Clone the repository.
2. Ensure the required libraries (mentioned above) are installed.
3. Run the cells of the attached `cnn-2-youssef.ipynb` Jupyter Notebook in order to observe the training results of each experiment and view the comparison plots.
