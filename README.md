# 🌱 Soil Moisture Binary Classification using ANN

This repository contains a beginner-friendly implementation of an **Artificial Neural Network (ANN)** built using **TensorFlow** and **Keras**. The model predicts whether a plant needs water based on environmental conditions like soil moisture, temperature, and sunlight exposure.

---

## 🚀 Project Overview

The objective of this project is to demonstrate the fundamentals of **Deep Learning for binary classification**:

* Data preprocessing and feature scaling
* Building a neural network using Sequential API
* Understanding activation functions (ReLU, Sigmoid)
* Training and evaluating a model
* Avoiding overfitting using validation data

---

## 📊 Dataset Description

The dataset consists of the following features:

| Feature                  | Description                     |
| ------------------------ | ------------------------------- |
| **Soil Moisture**        | Water content in soil (float)   |
| **Temperature (°C)**     | Ambient temperature             |
| **Sunlight Hours**       | Daily sunlight exposure         |
| **Needs Water (Target)** | Binary output (1 = Yes, 0 = No) |

---

## 🧠 Model Architecture

This is a **Feedforward Neural Network (ANN)**:

```
Input Layer (3 features)
        ↓
Dense Layer (8 neurons, ReLU)
        ↓
Output Layer (1 neuron, Sigmoid)
```

### 🔹 Explanation:

* **ReLU Activation** → Introduces non-linearity
* **Sigmoid Activation** → Outputs probability (0–1)
* **Dense Layers** → Fully connected layers

---

## ⚙️ Training Configuration

| Parameter     | Value               |
| ------------- | ------------------- |
| Optimizer     | sgd               |
| Loss Function | Binary Crossentropy |
| Metrics       | Accuracy            |
| Epochs        | 100                 |
| Batch Size    | 4                   |

---

## 🛠️ Tech Stack

* **Language:** Python
* **Libraries:**

  * TensorFlow / Keras → Model building
  * Pandas → Data handling
  * Scikit-learn → Train-test split & preprocessing

---

## 📂 How to Run the Project

### 1️⃣ Clone the repository

```bash
git clone https://github.com/sumran58/ann_base_model.git
```

### 2️⃣ Navigate to project

```bash
cd repository-name
```

### 3️⃣ Install dependencies

```bash
pip install tensorflow pandas scikit-learn matplotlib
```

### 4️⃣ Run the notebook

Open `.ipynb` file in:

* Google Colab OR
* Jupyter Notebook

---

## 📈 Model Training Visualization (Recommended)

Add this code to visualize training:

```python
import matplotlib.pyplot as plt

plt.plot(history.history['loss'], label='Train Loss')
plt.plot(history.history['val_loss'], label='Validation Loss')
plt.legend()
plt.xlabel("Epochs")
plt.ylabel("Loss")
plt.title("Training vs Validation Loss")
plt.show()
```

---

## 📊 Sample Output

* Model predicts probability:

  * **> 0.5 → Needs Water 🌱**
  * **< 0.5 → No Water Needed**

---

## 🚀 Future Improvements

* 🔹 Use **StandardScaler** for better normalization
* 🔹 Add more hidden layers (Deep Learning)
* 🔹 Use **Dropout** to reduce overfitting
* 🔹 Hyperparameter tuning (learning rate, batch size)
* 🔹 Deploy model using Flask / FastAPI

---

## 💡 Key Learnings

* Importance of feature scaling
* Role of activation functions
* Understanding training vs validation performance
* Basics of ANN architecture

---

## 📌 Best Practices for GitHub

* ✅ Add `model.summary()` screenshot
* ✅ Upload training graph
* ✅ Add `.gitignore` file
* ✅ Include LICENSE (MIT recommended)

---

## 📜 License

This project is open-source and available under the **MIT License**.

---

## 🙌 Acknowledgment

This project is part of a learning journey in **Artificial Intelligence and Data Science**, focusing on building real-world ML/DL projects.

---

⭐ If you found this helpful, consider giving this repo a star!
