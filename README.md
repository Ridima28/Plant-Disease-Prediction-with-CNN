# 🌿 Plant Disease Prediction with CNN

A Convolutional Neural Network that classifies plant leaf images into healthy / diseased categories.

## Overview
- **Task:** Multi-class image classification of plant leaf diseases
- **Model:** CNN built with `<TensorFlow/Keras> `
- **Dataset:** `< PlantVillage>` — `<N>` images, `<K>` classes
- **Result:** `93.17%` on the held-out test set

## Repository Structure
```
├── notebook.ipynb   # Data loading, preprocessing, training, evaluation
└── README.md
```

## Dataset
- Source: `https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset`
- Classes: ` Tomato___Late_blight, Potato___healthy, ...>`
- Split: `80-20`
- Image size: `224x224`

## Methodology
1. **Preprocessing:** resizing, normalization, 
2. **Model architecture:** `< 5 × Conv2D + MaxPool → Flatten → Dense(256) → Dropout → Softmax>`
3. **Training:** optimizer `<Adam>`, loss `<categorical_crossentropy>`, epochs `<30>`, batch size `<32>`
4. **Evaluation:** accuracy

## Results
| Metric | Train |  Test |
|---|---|---|---|
| Accuracy | `<97%>` | `<93%>` |


## Getting Started
```bash
git clone https://github.com/Ridima28/Plant-Disease-Prediction-with-CNN.git
cd Plant-Disease-Prediction-with-CNN
pip install tensorflow numpy pandas matplotlib scikit-learn
jupyter notebook notebook.ipynb
```
Or open directly in Google Colab and run all cells (GPU runtime recommended).

## Requirements
- Python 3.9+
- `<tensorflow / torch>`, numpy, pandas, matplotlib, scikit-learn

## Future Work
- Transfer learning (MobileNetV2 / EfficientNet)
- Deploy as a web app (Flask/Streamlit) for farmers
- Grad-CAM for explainability

## Author
**Ridima** — [GitHub](https://github.com/Ridima28)
