This project uses a CNN model to classify digits (0–9) with high accuracy. It includes the following key features:
- Integration with Kaggle for downloading and submitting datasets.
- Detailed data preprocessing and analysis.
- A custom CNN model with performance monitoring.
- Submission of results to a Kaggle competition.

## Workflow

The notebook is divided into the following stages:

| Step | Description                                                                                       |
|------|---------------------------------------------------------------------------------------------------|
| 1    | Import necessary libraries and setup Kaggle API credentials.                                     |
| 2    | Download and preprocess the MNIST dataset.                                                       |
| 3    | Analyze the dataset with visualizations to understand label distribution and data properties.     |
| 4    | Define and train a Convolutional Neural Network (CNN) model.                                      |
| 5    | Evaluate model performance and visualize results.                                                 |
| 6    | Make predictions on the test dataset and prepare a Kaggle submission file.                        |

---

## Key Steps

### 1. **Data Loading and Exploration**
- Dataset: MNIST (handwritten digit images).
- Preprocessing: Normalization, reshaping, and one-hot encoding.
- Visualizations:
  - Label distribution count plot.
  - Pixel intensity histograms.

### 2. **Model Architecture**
- A custom CNN with the following layers:
  - Convolutional layers with ReLU activation.
  - MaxPooling layers for dimensionality reduction.
  - Dropout for regularization.
  - Dense layers for classification.
- Optimizer: Adam.

### 3. **Training**
- Batch size: 50
- Epochs: 10
- Early stopping callback to terminate training once the desired accuracy is achieved.

### 4. **Evaluation**
- Metrics: Accuracy and loss over epochs.
- Visualization: Training and validation accuracy/loss curves.

### 5. **Submission**
- Predictions are saved in a CSV file and submitted to the Kaggle competition.

## Results

The trained CNN achieved the following performance:
- Training Accuracy: 98.7%
- Test Accuracy: 98.3%
- Confusion matrix visualizations to analyze misclassifications.
