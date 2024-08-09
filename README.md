# MNIST Image Classification 🧑🏼‍💻🔢🚀

![image](https://github.com/user-attachments/assets/41f9e668-6b01-4ebc-8250-786d9b3f98f7)

This project demonstrates various machine learning techniques for classifying handwritten digits from the MNIST dataset. It covers data preprocessing, model training, evaluation, and advanced classification strategies.

## Table of Contents

- [Project Overview](#project-overview)
- [Setup and Installation](#setup-and-installation)
- [Data Overview](#data-overview)
- [Data Visualization](#data-visualization)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Multi-Class Classification](#multi-class-classification)
- [Multi-Label Classification](#multi-label-classification)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The project focuses on image classification using the MNIST dataset, which contains 70,000 grayscale images of handwritten digits. We explore binary classification for detecting a specific digit, multiclass classification for all digits, and multi-label classification for scenarios where multiple labels may apply.

## Setup and Installation

To get started, clone the repository and install the required Python libraries. The project uses libraries like NumPy, pandas, Matplotlib, Scikit-learn, and Seaborn for data manipulation, visualization, and modeling. Follow the instructions in the [setup script](setup.py) to install dependencies.

## Data Overview

The MNIST dataset consists of 60,000 training images and 10,000 test images, each of size 28x28 pixels. Each image is labeled with a digit from 0 to 9. The dataset is well-balanced, though some digits are slightly more frequent than others.

## Data Visualization

We visualized individual and multiple digits from the dataset to understand the data better. Examples include displaying a single digit as a heatmap and plotting multiple digits in a grid to observe their variations.

## Model Training

### Binary Classification

Initially, we focused on a binary classification task to detect the digit '5' using the `SGDClassifier`. We transformed the labels into binary format and trained the model. A dummy classifier was used as a baseline for comparison.

### Multiclass Classification

We extended the classification problem to handle all ten digits using the `SVC` (Support Vector Classifier) and the `RandomForestClassifier`. Techniques like one-vs-one and one-vs-all strategies were used to manage multiple classes.

## Model Evaluation

### Performance Metrics

We evaluated the models using accuracy, precision, recall, and F1-score. Precision-recall curves and ROC curves were plotted to visualize the trade-offs and overall performance of different classifiers.

### Cross-Validation

Cross-validation was employed to assess the robustness of the models. We used methods like `cross_val_score` and `cross_val_predict` to obtain reliable performance metrics and validate the models' effectiveness.

## Multi-Class Classification

For the MNIST dataset, we implemented both one-vs-one and one-vs-all strategies. We used `SVC` and `RandomForestClassifier` to handle multi-class classification, analyzing the performance of each method.

## Multi-Label Classification

We explored multi-label classification by creating labels for digits greater than or equal to 7 and odd digits. The `KNeighborsClassifier` was used for this task, and the performance was evaluated using metrics like the F1-score.

## Contributing

Contributions to this project are welcome! Please submit issues, pull requests, or suggestions for improvements. Ensure that your contributions align with the project's goals and coding standards.

