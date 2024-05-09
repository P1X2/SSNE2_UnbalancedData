# House Value Prediction using MLP

This project focuses on predicting house values using a Multi-Layer Perceptron (MLP) model. The dataset used is both unbalanced and noisy, requiring significant pre-processing. 
Multiple normalization techniques are used to improve model performance. The final model achieves an accuracy of 86% on the test set. That is university project for neural network course.

## Project Overview

### Problem Statement
- **Task**: Predicting house values(class) based on various features using a multi-layer perceptron (MLP).
- **Dataset**: Contains features related to house attributes, location, and market conditions.

### Solution
- **Model Architecture**: A multi-layer perceptron (MLP) architecture with dropout, batch normalization, weight decay, and learning rate scheduling.
- **Key Features**:
  - Extensive data pre-processing, including normalization and covariance analysis.
  - Implementation of an MLP model tailored for noisy and unbalanced data.
  - Use of regularization techniques like dropout, batch normalization, and weight decay.

### Data Pre-Processing
1. **Covariance Analysis**:
   - Compute feature covariance to identify multicollinearity.
   - Remove redundant or highly correlated features.

2. **Normalization Techniques**:
   - Standardize features to have zero mean and unit variance.
   - Handle missing data and outliers with imputation techniques.

### Model Implementation
1. **Model Architecture**:
   - Input layer: Based on the number of features in the dataset.
   - Hidden layers: Multiple layers with ReLU activation, dropout, and batch normalization.
   - Output layer: Single output node for regression.

2. **Regularization Techniques**:
   - **Dropout**: Randomly drop nodes during training to prevent overfitting.
   - **Batch Normalization**: Normalize layer outputs for more stable training.
   - **Weight Decay**: Apply L2 regularization to model weights.

3. **Optimization**:
   - Optimizer: Adam optimizer with a learning rate scheduler.
   - Loss Function: Cross Entropy Loss

### Training Process
1. **Training Configuration**:
   - Batch size, learning rate, and epochs are configured through command-line arguments.
   - Model training with checkpointing and early stopping.

2. **Learning Rate Scheduler**:
   - One Cycle LR Scheduler

### Results
- **Accuracy**: 86% accuracy on the test set after implementing the MLP model with normalization techniques.
