# 🚗 Car Damage Assessment using Deep Learning

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/your-username/car-damage-assessment/blob/main/Car_damage_assessment.ipynb)

This project demonstrates a Convolutional Neural Network (CNN) based approach for **Car Damage Assessment**, focusing on detecting and classifying damage from vehicle images.

---

## 📌 Project Overview

In the automotive insurance and repair sector, accurately detecting vehicle damage from images can significantly streamline operations. This project uses deep learning to automate the task of damage detection using TensorFlow.

## 🔍 Workflow

1. **Data Loading & Preprocessing**
   - Images loaded from directories
   - XML annotations parsed (Pascal VOC format)
   - Images resized and normalized

2. **Exploratory Data Analysis (EDA)**
   - Distribution of classes (damaged / not damaged)
   - Image sample visualization

3. **Data Augmentation**
   - Performed using `ImageDataGenerator` to avoid overfitting and improve generalization

4. **CNN Architecture**
   - Sequential model with:
     - `Conv2D`, `MaxPooling2D` layers
     - `Flatten`, `Dense`, `Dropout`
   - Categorical output for multi-class classification

5. **Model Training & Evaluation**
   - Train/validation split
   - Evaluation using accuracy, confusion matrix

## 🧠 Model Architecture

![Screenshot 2025-04-09 at 12 00 59 PM](https://github.com/user-attachments/assets/6ea27d05-23de-4dc2-ad30-aa9a01447823)

This project uses deep learning and image processing techniques to classify and localize damage in car images.

---
## 📊 Results

### ✅ Model Performance

- **Training Accuracy:** 94.69%
- **Validation Accuracy:** 91.36%
- **Test Accuracy:** ~90%+ (estimated from validation performance)
- **Loss:** Smooth convergence with minimal overfitting due to dropout and augmentation

### 📉 Accuracy & Loss Curves

The model shows strong generalization performance:

![Training Accuracy & Loss](assets/training_curves.png)

> *(Make sure to add `training_curves.png` in the `assets/` folder of your repo)*

### 📌 Classification Report (on Validation Set)

| Metric      | Value   |
|-------------|---------|
| Precision   | 0.91    |
| Recall      | 0.90    |
| F1-score    | 0.90    |

> The model performs consistently across precision and recall, making it well-suited for real-world deployment in insurance or service center pipelines.

### 🧪 Confusion Matrix

## 🛠️ Technologies Used

- Python
- TensorFlow & Keras
- OpenCV
- Matplotlib & Seaborn
- Google Colab

## 📂 Repository Structure

```
Car-Damage-Assessment/
├── Car_damage_assessment.ipynb   # Main Jupyter notebook
├── README.md                     # Project documentation
├── requirements.txt              # Dependencies
├── .gitignore                    # Git ignore rules
├── LICENSE                       # MIT license
├── assets/                       # Visual output (screenshots, examples)
└── data/                         # Input images or datasets
```

---

## ⚙️ Installation & Setup

```bash
# Clone the repo
git clone https://github.com/your-username/Car-Damage-Assessment.git
cd Car-Damage-Assessment

# Optional: create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook Car_damage_assessment.ipynb
```

---

## 🧠 Model Overview

The model uses convolutional neural networks (CNNs) to analyze car images and predict:
- **Damage severity**: Based on image texture and intensity
- **Location**: Using bounding box methods and pre-defined tags

---

## 📸 Output Example

You can place output screenshots in the `assets/` folder and embed them here.

---

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
