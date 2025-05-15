## 🥔 Potato Leaf Disease Classification with CNN

This project uses Convolutional Neural Networks (CNN) to detect and classify diseases in potato leaves using the **PlantVillage dataset**. It includes data extraction, preprocessing, model building, training, and prediction.

---

### 📌 Table of Contents

* [Overview](#overview)
* [Dataset](#dataset)
* [Setup & Installation](#setup--installation)
* [How to Run](#how-to-run)
* [Model Architecture](#model-architecture)
* [Results](#results)
* [Technologies Used](#technologies-used)
* [License](#license)

---

### 🧠 Overview

Potato diseases can significantly impact crop yield. This project leverages CNN models to classify potato leaf images into:

* Healthy
* Early Blight
* Late Blight

---

### 📁 Dataset

* Source: [PlantVillage Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)
* Path after extraction: `/content/PlantVillage/PlantVillage`
* Classes: 3 (Healthy, Early Blight, Late Blight)

---

### 🛠️ Setup & Installation

1. Clone this repo:

   ```bash
   git clone https://github.com/Mohan5488/potato-disease-classification.git
   cd potato-disease-classification
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Upload the dataset to `/content/drive/MyDrive/PlantVillage.zip`

---

### 🚀 How to Run

1. Open the Jupyter notebook:

   ```bash
   jupyter notebook Potatao.ipynb
   ```

2. Make sure to mount Google Drive and unzip the dataset:

   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

3. Follow the cells to preprocess the data, build and train the CNN model.

---

### 🧱 Model Architecture

* Input: Resized 64x64 images
* Convolution + MaxPooling layers
* Flatten → Dense Layers
* Output Layer: 3 classes with softmax activation

---

### 📊 Results

* Accuracy: 0.979
* Loss: 0.068
* Model performs well on test data and distinguishes between disease types.

---

### 🧰 Technologies Used

* Python
* TensorFlow / Keras
* Google Colab
* Matplotlib & Seaborn
* OpenCV
* Pandas & NumPy
