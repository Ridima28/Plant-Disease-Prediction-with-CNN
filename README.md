
# 🌿 Plant Disease Prediction with CNN

A Convolutional Neural Network (CNN) that classifies plant leaf images into healthy and diseased categories.

## Overview

- **Task:** Multi-class image classification of plant diseases
- **Model:** CNN built with TensorFlow/Keras
- **Dataset:** [PlantVillage Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset)
- **Test Accuracy:** 93.17%


## Dataset

- **Source:** [Kaggle — PlantVillage Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset)
- **Classes:** Multiple plant disease categories, including `Tomato___Late_blight` and `Potato___healthy`
- **Image Size:** 224 × 224 pixels
- **Data Split:** 80% training and 20% validation/testing, as configured in the notebook

## Methodology

### Preprocessing
- Resize images to 224 × 224 pixels.
- Normalize pixel values.
- Split the dataset into training and validation/testing sets.

### Model Architecture

CNN architecture consisting of convolutional and pooling layers, followed by fully connected layers:

`Conv2D → MaxPooling2D → Flatten → Dense(256) → Dropout → Softmax`

*Update this description to match your actual model architecture.*

### Training Configuration

- **Optimizer:** Adam
- **Loss Function:** Categorical cross-entropy
- **Epochs:** 30
- **Batch Size:** 32

## Results

| Metric   | Training | Test   |
|----------|----------|--------|
| Accuracy | 97%      | 93.17% |

*Training accuracy is listed as 97% based on the current project notes. Verify both values against your actual evaluation results.*

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Ridima28/Plant-Disease-Prediction-with-CNN.git
cd Plant-Disease-Prediction-with-CNN
```

### 2. Install Dependencies

```bash
pip install tensorflow numpy pandas matplotlib scikit-learn
```

### 3. Run the Notebook

```bash
jupyter notebook notebook.ipynb
```

Alternatively, open the notebook in Google Colab, select a GPU runtime if available, and run the cells in order.

## Requirements

- Python 3.9+
- TensorFlow
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Future Work

- Explore transfer learning with MobileNetV2 or EfficientNet.
- Deploy the model as a web application using Flask or Streamlit.
- Integrate Grad-CAM for model explainability.
- Evaluate the model on real-world leaf images under different lighting conditions.

## Author

**Ridima**

[GitHub Repository](https://github.com/Ridima28/Plant-Disease-Prediction-with-CNN)
