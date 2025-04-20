# CNN Architecture Analysis Report

## LeNet Model

### 1. Introduction
LeNet-5 is one of the earliest CNN architectures, primarily designed for digit recognition. This section evaluates its performance on the dataset in terms of accuracy, efficiency, and complexity.

### 2. Model Summary
- **Total Parameters**: 133,280  
- **Trainable Parameters**: 44,426  
- **Non-trainable Parameters**: 0  
- **Test Accuracy**: 97.94%  
- **Layer Breakdown**:
  - Convolutional Layers: 2  
  - Pooling Layers: 2 (AveragePooling2D)  
  - Fully Connected Layers: 3

### 3. Performance Analysis
- **Strengths**:
  - Lightweight and suitable for low-resource environments
  - Simple and easy to debug
- **Weaknesses**:
  - Limited depth and feature extraction compared to modern models

### 4. Conclusion
LeNet provides reliable accuracy for simple tasks with minimal resources. It’s a solid option where efficiency is prioritized over complexity.

---

## VGG16 Model

### 1. Introduction
VGG16 is a deep CNN known for its simplicity and robust feature extraction.

### 2. Model Summary
- **Total Parameters**: 44,545,850  
- **Trainable Parameters**: 14,848,616  
- **Non-trainable Parameters**: 0  
- **Test Accuracy**: 98.56%  
- **Layer Breakdown**:
  - Convolutional Layers: 13  
  - Pooling Layers: 5 (MaxPooling2D)  
  - Fully Connected Layers: 2

### 3. Performance Analysis
- **Strengths**:
  - Strong feature extraction and generalization
  - Ideal for complex datasets
- **Weaknesses**:
  - High memory and computation needs
  - Risk of overfitting on small datasets

### 4. Conclusion
VGG16 is excellent for high-accuracy tasks but may not suit resource-limited settings.

---

## Comparative Analysis

### 1. Introduction
This section compares three models: LeNet, VGG16, and a custom Previous Architecture.

### 2. Test Accuracy & Parameters
- **Previous Architecture**: 98.93%, 279,968 parameters  
- **VGG16**: 98.56%, 44,545,850 parameters  
- **LeNet**: 97.94%, 133,280 parameters

### 3. Comparison
- **Accuracy**: Previous Architecture > VGG16 > LeNet  
- **Complexity**:
  - VGG16: Most complex
  - Previous: Balanced
  - LeNet: Most efficient
- **Efficiency**:
  - LeNet is the most efficient
  - Previous Architecture provides a good trade-off
  - VGG16 is resource-intensive
- **Generalization**:
  - VGG16 and Previous Architecture show better generalization
  - LeNet is suitable for small-scale problems

### 4. Conclusion
The Previous Architecture is the optimal choice balancing accuracy and efficiency. VGG16 excels in complex tasks, while LeNet remains a good option for lightweight applications.
