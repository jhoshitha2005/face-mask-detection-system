# Face Mask Detection Using Deep Learning

## 1. Introduction

This project implements a face mask detection system using deep learning and image classification techniques. It classifies facial images into two categories: **With Mask** and **Without Mask**.

The project uses a MobileNetV2-based convolutional neural network with TensorFlow and Keras to build an efficient image classification model.

## 2. Problem Statement

To develop a supervised machine learning model that can automatically classify facial images based on whether a person is wearing a face mask.

## 3. Type of Machine Learning Problem

- **Learning Type:** Supervised Learning
- **Task:** Binary Image Classification

**Classification Categories:**
- With Mask
- Without Mask

## 4. Dataset Description

The dataset contains facial images organised into two classes:

- With Mask
- Without Mask

The dataset is stored in Google Drive and accessed through Google Colab.

The images are divided into training and validation sets using an 80:20 split.

## 5. Data Preprocessing

The following preprocessing techniques were applied:

- Resizing images to 224 × 224 pixels.
- Converting images into RGB format.
- Applying MobileNetV2 preprocessing.
- Splitting the dataset into training and validation sets.
- Applying data augmentation techniques to improve model generalisation.

Data augmentation includes:
- Rotation
- Zoom
- Width and height shifting
- Shearing
- Horizontal flipping

## 6. Model Architecture

The project uses **MobileNetV2**, a lightweight convolutional neural network originally trained on ImageNet.

Transfer learning is applied by:

- Using MobileNetV2 as the base feature extraction model.
- Freezing the pretrained base model layers.
- Adding a Global Average Pooling layer.
- Adding a Dense layer with 128 neurons and ReLU activation.
- Using a final Dense layer with sigmoid activation for binary classification.

## 7. Model Training

The model is trained using TensorFlow and Keras.

Training configuration:

- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Evaluation Metric: Accuracy
- Batch Size: 32
- Maximum Epochs: 10
- Early Stopping: Enabled

Early stopping is used to prevent unnecessary training and reduce overfitting.

## 8. Model Evaluation

The model is evaluated using the validation dataset.

Evaluation metrics and visualisations include:

- Training Accuracy
- Validation Accuracy
- Training Loss
- Validation Loss
- Classification Report
- Confusion Matrix

**Validation Accuracy: Approximately 98%**

## 9. System Workflow

The project follows this workflow:

1. Load the facial image dataset.
2. Preprocess and resize the images.
3. Apply data augmentation to training images.
4. Extract image features using MobileNetV2.
5. Train the binary classification model.
6. Evaluate model performance using validation data.
7. Predict whether an uploaded image contains a person wearing a mask.

## 10. Results and Visualisation

The notebook includes:

- Model accuracy and loss graphs.
- Confusion matrix.
- Classification report.
- Image-based prediction functionality.

These results help evaluate the model's classification performance.

## 11. Tools and Technologies Used

- Python
- TensorFlow
- Keras
- MobileNetV2
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab
- Google Drive

## 12. Conclusion

This project demonstrates the application of deep learning and transfer learning for face mask classification.

By using MobileNetV2 and TensorFlow, the system can classify facial images into masked and unmasked categories. The project provided practical experience in dataset preparation, image preprocessing, model training, evaluation and computer vision workflows.

## 13. Course Outcome Mapping

- **CO1:** Identified suitable machine learning techniques.
- **CO2:** Applied machine learning to a real-world classification problem.
- **CO3:** Developed a deep learning-based application.
- **CO4:** Evaluated and interpreted model performance.

## 14. Future Enhancements

- Extend the dataset with more diverse facial images.
- Introduce a third class for incorrectly worn masks.
- Integrate face detection for processing images containing multiple faces.
- Develop a real-time detection application using a webcam.
- Deploy the model as a web or mobile application.

---

**Author:** Jhoshitha Myneni

**Project:** Face Mask Detection Using Deep Learning
