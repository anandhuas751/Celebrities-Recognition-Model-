# Celebrities-Recognition-Model-
# Celebrities Recognition Model Readme

## Overview

### Model

**Selected Model:** Convolutional Neural Network (CNN)

#### Architecture

- **Input Layer:** Supports 128x128 pixel images with 3 color channels.
  
- **Convolutional Layer:** (3, 3) kernel, ReLU activation, 32 filters.

- **Max Pooling Layer:** Efficient feature extraction.

- **Flatten Layer:** Vector representation of 2D matrix data.

- **Dense Layers:** ReLU activation, one layer with 0.1 dropout. Softmax activation in the last layer for multi-class classification.

#### Compilation

- **Optimizer:** Adam optimizer.

- **Loss Function:** Sparse categorical crossentropy for integer labels in multi-class classification.

#### Training Procedure

**Data Loading and Preprocessing:**
Reads and preprocesses images from a designated directory, resizing to 128x128 pixels, and normalizing pixel values.

**Data Splitting:**
70% training, 30% testing.

**Model Training:**
20 epochs, batch size 128, with 10% validation split.

**Visualizations:**
Generates and saves accuracy and loss plots for training and validation sets.

## Critical Findings

### Accuracy and Loss Plots

- **Accuracy Plot:** Incremental improvement over epochs for training and validation datasets.

- **Loss Plot:** Illustrates model generalization by showing convergence during training.

### Model Evaluation

- Uses a separate test set for evaluating the trained model's performance.

- Prints accuracy on the test data.

### Example Predictions

- Showcases model predictions on images of celebrities: Lionel Messi, Roger Federer, Virat Kohli, Maria Sharapova, and Serena Williams.

- Provides a qualitative assessment of the model's real-world performance.

*Note: Some predictions may be incorrect due to misleading images in certain folders within the training set.*

## Conclusion

The CNN model exhibits promise in identifying celebrities. Key findings, including loss and accuracy graphs, offer insights into the learning dynamics. Real-world performance is assessed through test set evaluation and example predictions. Opportunities for optimization and improvement are identified to enhance precision and resilience.
