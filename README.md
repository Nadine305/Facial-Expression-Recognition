# Facial Expression Recognition

This project classifies facial expressions into one of seven emotion categories using classical computer vision techniques and machine learning.

## 📁 Emotion Labels

* **0**: Angry
* **1**: Disgust
* **2**: Fear
* **3**: Happy
* **4**: Sad
* **5**: Surprise
* **6**: Neutral

---

## 📦 Dataset

We use the [FER-2013 dataset](https://www.kaggle.com/datasets/msambare/fer2013) from Kaggle, which provides labeled 48x48 grayscale facial images.

---

## 🧼 Preprocessing Pipeline

Each image is enhanced using:

* CLAHE (Contrast Limited Adaptive Histogram Equalization)
* Gaussian denoising
* Histogram stretching
* Gamma correction
* Sharpening
* Normalization

---

## 🔄 Data Augmentation

Augmentations include:

* Horizontal flip
* Rotation (+15°)
* Brightness adjustment (selective)

---

## 🧠 Feature Extraction

We extract and combine:

* **HOG** (Histogram of Oriented Gradients) features
* **LBP** (Local Binary Patterns)

---

## 🧪 Dimensionality Reduction

* Features are scaled with `StandardScaler`
* Reduced using **PCA** to 300 components

---

## 📊 Classification

Tested models:

* SVM (RBF)
* Random Forest (best performance)
* KNN
* MLP (Multi-layer Perceptron)

Evaluation includes accuracy and confusion matrix visualization.

---

## 📉 Handling Imbalance

Used `RandomUnderSampler` from **imbalanced-learn** to balance classes in the training set.

---

## 🖼️ Visualizations

* Class distribution before and after resampling
* Original vs. preprocessed image comparison
* HOG and LBP visualizations

---

## 📌 Usage

1. Download dataset from Kaggle using `kagglehub`
2. Run preprocessing and feature extraction
3. Train and evaluate with your preferred classifier
