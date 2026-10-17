# Handwritten Digit Detection and Localization

## Overview
This project uses a Convolutional Neural Network (CNN) to classify handwritten digits and predict their bounding boxes in images.

Unlike a standard digit classifier, this model performs two tasks:
- **Digit Classification:** Predicts the digit from 0 to 9.
- **Bounding Box Regression:** Predicts the location of the digit using four coordinates.

## Technologies Used
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- TensorFlow Datasets (TFDS)

## Model Architecture
The model uses a shared CNN feature extractor with two output heads:
1. **Classification Head:** Uses Softmax to predict one of 10 digit classes.
2. **Bounding Box Regression Head:** Uses Sigmoid to predict four normalized bounding box coordinates.

The model is trained using:
- Categorical Cross-Entropy for classification.
- Mean Squared Error (MSE) for bounding box regression.
- Adam optimizer.

## Results

| Metric | Result |
|---|---:|
| Mean Intersection over Union (IoU) | 0.8110 |
| Bounding Boxes with IoU ≥ 0.5 | 99.99% |

*Results are from the notebook's validation evaluation.*

## How to Run
1. Clone this repository.
2. Install the required dependencies.
3. Open `Object_Detection.ipynb` in Jupyter Notebook or Google Colab.
4. Run the notebook cells in order.

## 📁 Project Structure
```text
Object-Detection/
├── Object_Detection.ipynb
└── README.md
```

## 👩‍💻 Author
Apurva Arya