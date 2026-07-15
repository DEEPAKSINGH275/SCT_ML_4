# ✋ Hand Gesture Recognition using Convolutional Neural Network (CNN)

## Overview

This project implements a **Convolutional Neural Network (CNN)** to recognize and classify different hand gestures from images. The model is trained on the **LeapGestRecog** dataset and is capable of accurately identifying **10 different hand gestures**, enabling gesture-based human-computer interaction systems.

The project demonstrates the complete deep learning pipeline, including image preprocessing, CNN model development, training, evaluation, and visualization of predictions.

---

## Objective

The objective of this project is to develop a robust hand gesture recognition system that can accurately classify hand gestures from image data using a Convolutional Neural Network (CNN).

---

## Dataset

This project uses the **LeapGestRecog** dataset available on Kaggle.

**Dataset Link**

https://www.kaggle.com/datasets/gti-upm/leapgestrecog

### Dataset Information

- 10 Subjects
- 10 Hand Gesture Classes
- Approximately **20,000 Images**
- RGB Images
- Image size resized to **64 × 64 pixels**

### Gesture Classes

| Label | Gesture |
|--------|----------------|
| 01 | Palm |
| 02 | L |
| 03 | Fist |
| 04 | Fist Moved |
| 05 | Thumb |
| 06 | Index |
| 07 | OK |
| 08 | Palm Moved |
| 09 | C |
| 10 | Down |

---

## Technologies Used

- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

---

## Project Workflow

1. Downloaded the LeapGestRecog dataset from Kaggle.
2. Loaded images from all gesture classes.
3. Resized images to **64 × 64** pixels.
4. Converted images to RGB format.
5. Normalized pixel values.
6. Encoded gesture labels.
7. Split dataset into training and testing sets.
8. Built a CNN architecture.
9. Trained the CNN model.
10. Evaluated the model using multiple performance metrics.
11. Visualized predictions and confusion matrix.

---

## CNN Architecture

The model consists of:

- Conv2D (32 Filters)
- MaxPooling2D
- Conv2D (64 Filters)
- MaxPooling2D
- Conv2D (128 Filters)
- MaxPooling2D
- Flatten Layer
- Dense Layer (256 Neurons)
- Dropout (0.5)
- Output Layer (Softmax - 10 Classes)

---

## Image Preprocessing

The following preprocessing steps were performed:

- Image resizing to **64 × 64**
- RGB conversion
- Pixel normalization (0–1)
- One-hot encoding of labels
- Train-Test Split

---

## Model Training

- Optimizer : Adam
- Loss Function : Categorical Crossentropy
- Epochs : 10
- Batch Size : 32
- Validation Split : 20%

---

## Model Performance

### Test Accuracy

**99.92%**

### Classification Metrics

| Metric | Score |
|---------|--------|
| Accuracy | **99.92%** |
| Precision | **1.00** |
| Recall | **1.00** |
| F1-Score | **1.00** |

The model achieved near-perfect performance across all gesture classes.

---

## Evaluation Metrics

The following evaluation metrics were used:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report
- Confusion Matrix

---

## Visualizations

The notebook generates the following visualizations:

- Sample images from the dataset
- Training Accuracy Curve
- Validation Accuracy Curve
- Training Loss Curve
- Validation Loss Curve
- Confusion Matrix
- Sample Gesture Predictions

---

## Results

The CNN model achieved an outstanding **99.92% test accuracy** on the LeapGestRecog dataset.

The confusion matrix demonstrates that almost all hand gestures are classified correctly, while the classification report shows precision, recall, and F1-score close to **1.00** for every gesture class.

This indicates that the CNN architecture effectively learns discriminative visual features and generalizes well to unseen test images.

---

## Project Structure

```
Hand_Gesture_Recognition/
│
├── Hand_Gesture_Recognition_CNN.ipynb
├── README.md
├── requirements.txt
├── dataset_link.txt
├── Accuracy.png
├── Loss.png
├── Confusion_Matrix.png
├── Sample_Predictions.png
└── Saved_Model/
```

---

## Requirements

Install all required libraries using:

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install tensorflow
pip install numpy
pip install matplotlib
pip install opencv-python
pip install scikit-learn
pip install kaggle
```

---

## How to Run

1. Clone this repository.

```bash
git clone https://github.com/DEEPAKSINGH275/Your_Repository_Name.git
```

2. Open the notebook in Google Colab or Jupyter Notebook.

3. Download the dataset from Kaggle.

4. Extract the dataset.

5. Update the dataset path in the notebook.

6. Run all notebook cells.

7. View the evaluation metrics and generated visualizations.

---

## Future Improvements

- Implement Transfer Learning using MobileNetV2.
- Train deeper CNN architectures such as ResNet50 or EfficientNet.
- Perform real-time hand gesture recognition using a webcam.
- Deploy the trained model using Streamlit or Flask.
- Optimize the model for mobile and edge devices using TensorFlow Lite.

---

## Author

**Deepak Singh**

B.Tech Computer Science and Engineering

Dr. B. R. Ambedkar National Institute of Technology (NIT) Jalandhar

---

## Acknowledgements

- Kaggle
- LeapGestRecog Dataset
- TensorFlow
- OpenCV
- Scikit-learn
