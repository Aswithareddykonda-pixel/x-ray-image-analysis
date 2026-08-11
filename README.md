# 🩻 X-Ray Image Analysis Using Deep Learning

## 📌 Overview

X-Ray Image Analysis is an AI-based image classification project that uses Deep Learning and Convolutional Neural Networks (CNNs) to analyze chest X-ray images.

The system processes an uploaded X-ray image and classifies it into two categories:

* **NORMAL**
* **PNEUMONIA**

The project demonstrates how computer vision and deep learning can be applied to medical image analysis.

> ⚠️ **Disclaimer:** This project is intended for educational and research purposes only. It is not a medical diagnostic tool and should not be used to make clinical decisions.

---

## 🎯 Objectives

* Analyze chest X-ray images using Artificial Intelligence.
* Preprocess medical images for deep learning.
* Build a CNN image classification model.
* Classify X-ray images into NORMAL and PNEUMONIA.
* Display prediction confidence.
* Provide a simple web interface for image upload.
* Demonstrate the use of AI in medical image analysis.

---

## 🧠 How the System Works

```text
X-Ray Image
     ↓
Image Upload
     ↓
Image Preprocessing
     ↓
Resize to 224 × 224
     ↓
Pixel Normalization
     ↓
CNN Feature Extraction
     ↓
Classification
     ↓
NORMAL / PNEUMONIA
     ↓
Confidence Score
```

---

## 🏗️ Project Structure

```text
X-Ray-Image-Analysis/
│
├── dataset/
│   ├── train/
│   ├── validation/
│   └── test/
│
├── models/
│   └── xray_model.keras
│
├── static/
│   └── uploads/
│
├── templates/
│   └── index.html
│
├── train.py
├── predict.py
├── app.py
├── requirements.txt
├── accuracy_graph.png
├── loss_graph.png
├── confusion_matrix.png
├── README.md
└── .gitignore
```

---

## 🛠️ Technologies

* Python
* TensorFlow
* Keras
* OpenCV
* NumPy
* Matplotlib
* Scikit-learn
* Flask
* HTML/CSS
* Git
* GitHub

---

## 📊 Dataset

The project requires a labeled chest X-ray dataset containing NORMAL and PNEUMONIA images.

The dataset should be organized as:

```text
dataset/
├── train/
│   ├── NORMAL/
│   └── PNEUMONIA/
│
├── validation/
│   ├── NORMAL/
│   └── PNEUMONIA/
│
└── test/
    ├── NORMAL/
    └── PNEUMONIA/
```

Please follow the dataset provider's license and usage requirements.

---

## 🔬 Deep Learning Model

The project uses a Convolutional Neural Network containing:

1. Convolutional layers
2. ReLU activation
3. Max pooling
4. Feature extraction
5. Flatten layer
6. Dense layer
7. Dropout
8. Sigmoid output layer

The sigmoid output produces a probability used to determine the predicted class.

---

## 🚀 Installation

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Enter the project directory:

```bash
cd X-Ray-Image-Analysis
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Training

Run:

```bash
python train.py
```

The trained model will be saved in:

```text
models/xray_model.keras
```

The program also generates training graphs.

---

## 🔍 Prediction

To analyze a single image:

```bash
python predict.py sample_xray.jpg
```

Example output:

```text
-----------------------------
      X-RAY ANALYSIS
-----------------------------
Prediction : NORMAL
Confidence : 91.35%
-----------------------------
```

---

## 🌐 Web Application

Start the Flask application:

```bash
python app.py
```

Open the browser and visit:

```text
http://127.0.0.1:5000
```

Upload an X-ray image and click:

```text
Analyze X-Ray
```

The application displays the predicted class and confidence score.

---

## 📈 Results

The following metrics can be used to evaluate the model:

* Training Accuracy
* Validation Accuracy
* Test Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Test Loss

Actual values should be recorded from the model after training rather than manually entered.

Example:

```text
Training Accuracy   : XX.XX%
Validation Accuracy : XX.XX%
Test Accuracy       : XX.XX%
```

---

## 💡 Uses

This project can demonstrate applications such as:

* Medical image analysis research
* AI and healthcare education
* Computer vision learning
* Deep learning experimentation
* X-ray image classification
* Student academic projects
* AI prototype development

It should not be used as a substitute for professional medical diagnosis.

---

## 🔮 Future Improvements

### 1. Transfer Learning

Use pretrained models such as:

* MobileNetV2
* ResNet50
* EfficientNet
* DenseNet

This can potentially improve performance compared with a basic CNN.

### 2. Multi-Class Disease Detection

Instead of two classes, the system could be extended to identify multiple findings or conditions, depending on an appropriately labeled dataset.

### 3. Explainable AI

Add Grad-CAM or similar explainability techniques to highlight image regions that influenced the model's prediction.

### 4. Better User Interface

Create a modern dashboard with:

* Image preview
* Prediction
* Confidence
* Prediction history
* Model performance charts

### 5. Cloud Deployment

The application could be deployed using an appropriate cloud platform for demonstration purposes.

### 6. Model Optimization

Use:

* Data augmentation
* Hyperparameter tuning
* Class balancing
* Transfer learning
* Regularization

to improve generalization.

### 7. Larger Datasets

Training on larger, diverse, properly labeled datasets can help evaluate whether the model generalizes to different populations and imaging conditions.

---

## ⚠️ Limitations

* The model's performance depends heavily on the training dataset.
* Dataset bias can affect predictions.
* X-ray image quality can influence results.
* The model may not generalize to every hospital or imaging device.
* Confidence scores do not guarantee correctness.
* This prototype is not clinically validated.

---

## 🎓 Academic Value

This project demonstrates practical knowledge of:

* Machine Learning
* Deep Learning
* CNN
* Computer Vision
* Image Preprocessing
* Model Evaluation
* Flask
* Python
* GitHub

---

## 👩‍💻 Author

**Your Name**

B.Tech – Artificial Intelligence and Data Science

---

## ⭐ Disclaimer

This project is created for educational purposes. It should not be used for medical diagnosis, treatment decisions, or emergency healthcare decisions.
