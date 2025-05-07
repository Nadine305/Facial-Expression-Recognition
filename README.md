# Facial-Expression-Recognition
## Emotion Recognition Task

The task is to categorize each face based on the emotion shown in the facial expression into one of seven categories:

- 0 = Angry  
- 1 = Disgust  
- 2 = Fear  
- 3 = Happy  
- 4 = Sad  
- 5 = Surprise  
- 6 = Neutral
  
---
### 🔧 Preprocessing

We apply a series of image enhancements:

* CLAHE (contrast improvement)
* Denoising with Gaussian blur
* Histogram stretching
* Gamma correction
* Sharpening
* Normalization

---

### 📈 Data Augmentation

Each image is augmented using:

* Horizontal flip
* Rotation (±15°)
* Brightness adjustment

---

### 🧠 Feature Extraction

We use:

* **HOG (Histogram of Oriented Gradients)**
* **LBP ()**


---

### 📊 Visualizations

We provide:

* Original vs. preprocessed image comparison
* Class distribution plots

---


## Dataset

We use the [FER-2013 dataset](https://www.kaggle.com/datasets/msambare/fer2013) from Kaggle, which provides labeled facial expression data for training and evaluation.
