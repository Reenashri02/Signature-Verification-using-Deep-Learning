# Signature-Verification-using-Deep-Learning
Signature Verification using Deep Learning
# 🖋️ Signature Verification Using Deep Learning

## 📌 Project Overview

This project develops a **Deep Learning-based Signature Verification System** using a **Convolutional Neural Network (CNN)**.

The model analyzes signature images and classifies them into two classes:

* **Genuine**
* **Forgery**

The project includes image preprocessing, signer-wise data splitting, CNN model training, evaluation, confusion matrix analysis, classification report, and single-signature prediction.

## 🎯 Project Objectives

* Develop a deep learning model for signature verification.
* Classify signature images into genuine and forgery classes.
* Preprocess and normalize signature images for CNN-based learning.
* Automatically extract important visual patterns using CNN.
* Evaluate the model using accuracy, precision, recall, F1-score, and confusion matrix.
* Predict whether a new signature is genuine or forged.

## ❓ Problem Statement

Manual signature verification is time-consuming and may be difficult when signatures have small variations.

Therefore, this project aims to develop a deep learning-based system that can automatically distinguish between **genuine and forged signatures** from signature images.

## 🛠️ Technologies Used

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## 🔄 Project Workflow

1. Import Libraries
2. Load Dataset
3. Count Dataset Images
4. Visualize Signature Images
5. Image Preprocessing
6. CNN Input Shape Preparation
7. Signer-wise Data Splitting
8. Check Class Distribution
9. Build CNN Model
10. Compile CNN Model
11. Configure Training Callbacks
12. Create Train-Validation Split
13. Create Training, Validation and Test Data
14. Calculate Class Weights
15. Train CNN Model
16. Plot Training and Validation Performance
17. Evaluate Final CNN Model
18. Generate Confusion Matrix
19. Generate Classification Report
20. Perform Single Signature Prediction

## 🖼️ Image Preprocessing

The signature images are:

* Converted to grayscale.
* Resized to **128 × 128 pixels**.
* Normalized by dividing pixel values by **255**.
* Reshaped into CNN-compatible input format: **128 × 128 × 1**.

The classes are represented as:

* `0` → Genuine
* `1` → Forgery

## 🧠 CNN Model

A **Convolutional Neural Network (CNN)** is used to automatically learn visual patterns from signature images.

The model uses:

* Convolutional layers
* Max Pooling
* Batch Normalization
* Flatten layer
* Dense layers
* Dropout
* Binary classification output

The model is compiled using:

* **Optimizer:** Adam
* **Learning Rate:** 0.001
* **Loss Function:** Binary Crossentropy
* **Metric:** Accuracy

## ⚖️ Class Weights

Class weights are calculated during training to handle differences in the number of samples between the Genuine and Forgery classes.

This helps the CNN give appropriate importance to both classes during training.

## ⏱️ Training Callbacks

Two callbacks are used:

### Early Stopping

Monitors validation loss and stops training when the model stops improving, while restoring the best model weights.

### Reduce Learning Rate

Reduces the learning rate when validation performance stops improving, helping the model continue learning effectively.

## 📊 Model Evaluation

The final model is evaluated using:

* Test Accuracy
* Confusion Matrix
* Precision
* Recall
* F1-Score
* Classification Report

### Final Test Accuracy

**79.71%**

The model was evaluated on unseen signature images.

## 🔍 Single Signature Prediction

The trained CNN is also used to predict an individual signature image.

The system displays:

* Actual Label
* Predicted Label
* Prediction Probability

The prediction is classified as either **Genuine** or **Forgery**.

## 📌 Conclusion

The project successfully developed a **CNN-based Signature Verification System** capable of classifying signature images as genuine or forged.

The model achieved **79.71% test accuracy** on unseen signature images. The confusion matrix and classification report were used to understand the model's classification performance.

The system also successfully performed **single-signature prediction**, demonstrating its ability to classify an individual signature image.

## ⚠️ Project Limitations

* The model achieved 79.71% accuracy, so some signatures are still misclassified.
* Genuine signatures had 58% recall, meaning some genuine signatures were classified as forgery.
* The model was trained on a specific signature dataset, so performance may vary on completely different datasets.
* Image quality, size, and writing variations can affect prediction.

## 🚀 Future Enhancements

* Use a larger and more diverse signature dataset.
* Apply data augmentation to improve generalization.
* Experiment with transfer learning models such as MobileNet, ResNet, or EfficientNet.
* Improve the model's ability to recognize genuine signatures.
* Deploy the model as a web or mobile application for real-time signature verification.

## 👩‍💻 Submitted By

**Reena Shri**


