# BrainVision-AI
BrainVision AI is a Deep Learning-based brain MRI classification project developed to classify MRI images into four different categories: Glioma, Meningioma, Pituitary Tumor, and No Tumor.

The project focuses on applying Transfer Learning with MobileNetV2 and evaluating the model using multiple performance metrics such as accuracy, precision, recall, F1-score, and confusion matrix.

---

## 📌 Project Overview

Brain tumors are abnormal growths of cells in the brain that can differ in their characteristics and appearance in MRI scans.

The main objective of BrainVision AI is to develop a deep learning model that can analyze brain MRI images and classify them into the following categories:

- Glioma
- Meningioma
- Pituitary Tumor
- No Tumor

This project helped me explore the complete workflow of a Deep Learning image classification problem, from dataset preparation and preprocessing to model training and evaluation.

---

## 🎯 Objectives

- Build a Deep Learning model for brain MRI classification.
- Use Transfer Learning to improve image classification performance.
- Classify MRI images into four different categories.
- Create separate training, validation, and testing data.
- Evaluate the model using multiple classification metrics.
- Analyze model performance using a confusion matrix.
- Identify classes that are difficult for the model to distinguish.

---

## 🧠 Model Used

### MobileNetV2

The project uses **MobileNetV2** with Transfer Learning.

MobileNetV2 is a lightweight convolutional neural network architecture that was originally trained on the ImageNet dataset.

The pre-trained model is used as a feature extractor and additional classification layers are added for the brain MRI classification task.

### Model Workflow

```text
Brain MRI Image
       ↓
Image Preprocessing
       ↓
MobileNetV2
       ↓
Feature Extraction
       ↓
Classification Layers
       ↓
Softmax Output
       ↓
Predicted Brain Tumor Class


📊 Dataset

The project uses the BRISC 2025 Brain MRI Dataset for the classification task.

The classification problem contains four classes:

Glioma
Meningioma
Pituitary
No Tumor

The dataset provides separate training and testing data.

A validation set was created from the training data during model development so that the test set could remain independent for final evaluation.

⚙️ Data Preprocessing

The following preprocessing steps were performed:

Loaded MRI images from the dataset.
Resized images to the required input size.
Converted images to RGB format for compatibility with MobileNetV2.
Created training and validation splits.
Batched the dataset for efficient training.
Applied MobileNetV2-compatible preprocessing.

🔬 Model Training

The model was trained using TensorFlow and Keras.

The training process included:

Transfer Learning
Validation monitoring
Early Stopping
Best model weight restoration
Multi-class classification

Early Stopping was used to prevent unnecessary training when validation performance stopped improving.

📈 Model Evaluation

The model was evaluated using multiple metrics instead of relying only on accuracy.

The evaluation included:

Accuracy
Precision
Recall
F1-Score
Confusion Matrix

The confusion matrix was used to understand how well the model performed for each individual class and to identify common misclassifications.

One of the main challenges observed during experimentation was distinguishing between Glioma and Meningioma.

📊 Results

The model achieved approximately 87.8% accuracy on the test dataset during experimentation.

The model performance was further analyzed using precision, recall, F1-score, and the confusion matrix.

The results showed that some classes were easier for the model to classify, while Glioma and Meningioma were comparatively more challenging.

This demonstrates why evaluating a classification model using multiple metrics is important, especially for medical image classification.

🛠️ Technologies Used
Python
TensorFlow
Keras
MobileNetV2
NumPy
Matplotlib
Scikit-learn
Jupyter Notebook

🚀 Key Learning Outcomes

Through this project, I gained practical experience in:

Working with medical image datasets.
Image preprocessing using TensorFlow/Keras.
Transfer Learning.
Using pre-trained CNN architectures.
Training and validating Deep Learning models.
Handling multi-class image classification.
Evaluating models using precision, recall, and F1-score.
Understanding and interpreting confusion matrices.
Identifying model weaknesses instead of relying only on accuracy.


🔮 Future Improvements
Future improvements for BrainVision AI could include:

Training with larger and more diverse MRI datasets.
Experimenting with different CNN and Transfer Learning architectures.
Applying more advanced data augmentation techniques.
Improving classification performance for Glioma and Meningioma.
Adding Brain Tumor Segmentation.
Exploring Explainable AI techniques such as Grad-CAM.
Comparing multiple Deep Learning architectures.


⚠️ Disclaimer
This project is developed for educational and research purposes only.
The model should not be used as a replacement for professional medical diagnosis or clinical decision-making.

👨‍💻 Author
Siddesh S Kuppast

Developed as a Deep Learning and Computer Vision project to explore the application of neural networks and Transfer Learning to medical image classification.