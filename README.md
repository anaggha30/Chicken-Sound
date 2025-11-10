# 🐔 Chicken Sound Recognition & Classification System

[![Language](https://img.shields.io/badge/Language-Python-blue?logo=python)](https://www.python.org/)
[![Libraries](https://img.shields.io/badge/Libraries-Librosa%20%7C%20TensorFlow%20%7C%20Keras%20%7C%20NumPy-orange)]()
[![Environment](https://img.shields.io/badge/Environment-Jupyter%20Notebook-lightgrey?logo=jupyter)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

An **AI-powered sound analysis project** designed to recognize and classify **chicken vocalizations** such as feeding, distress, happiness, and nesting sounds.  
This project applies **audio feature extraction** and **machine learning** to help understand **behavioral and environmental patterns** in poultry farms.

---

## 🚀 Features

- 🔊 **Audio Classification:** Identifies different chicken sounds (e.g., happy, eating, distress, hungry).  
- 🧠 **Machine Learning Model:** Uses a CNN/LSTM-based sound classification model.  
- 📊 **Audio Feature Extraction:** Extracts features like **MFCC**, **spectrogram**, and **chroma**.  
- 🎧 **Dataset Handling:** Prepares `.wav` sound files into train-test datasets.  
- 🐣 **Behavior Monitoring:** Provides insights into chicken welfare and activity through sound analysis.  
- 💾 **Efficient Storage:** Supports multiple `.wav` files organized by categories.  

---

## 🧰 Tech Stack

### 🧠 Tools & Libraries
- **Programming Language:** Python  
- **Libraries:** Librosa, NumPy, Pandas, TensorFlow/Keras, Matplotlib, Scikit-learn  
- **Environment:** Jupyter Notebook / Google Colab  

---

## 🏗️ Project Architecture

```text
 ┌────────────────────────────┐
 │     Audio Dataset (.wav)   │
 │  (Happy, Eating, Hungry...)│
 └────────────┬───────────────┘
              │
              ▼
 ┌────────────────────────────┐
 │   Audio Feature Extraction │
 │  (MFCC, Spectrogram, etc.)│
 └────────────┬───────────────┘
              │
              ▼
 ┌────────────────────────────┐
 │   Model Training (CNN/LSTM)│
 │  Classification + Validation│
 └────────────┬───────────────┘
              │
              ▼
 ┌────────────────────────────┐
 │     Sound Prediction App   │
 │  Identify chicken behavior │
 └────────────────────────────┘
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/anaggha30/Chicken-Sound.git
cd Chicken-Sound
```

### 2️⃣ Install Required Libraries
```bash
pip install numpy pandas librosa tensorflow scikit-learn matplotlib
```

### 3️⃣ Run the Jupyter Notebook
```bash
jupyter notebook Chicken_Sound_Analysis.ipynb
```

### 4️⃣ Add Your Dataset
Place your `.wav` files inside folders (e.g. `happy/`, `eating/`, `hungry/`) under a directory named **dataset**:
```
dataset/
 ├── happy/
 ├── eating/
 ├── hungry/
 ├── unclassified/
 └── unknown/
```

---

## 📊 Sample Outputs

| Visualization | Description |
|----------------|--------------|
| ![Spectrogram](assets/spectrogram.png) | Spectrogram of chicken call frequency |
| ![Model Accuracy](assets/training_accuracy.png) | Model training accuracy and loss curves |
| ![Confusion Matrix](assets/confusion_matrix.png) | Model performance across sound categories |

---

## 🧠 Model Summary
- **Architecture:** CNN (Conv1D) / LSTM hybrid network  
- **Input:** MFCC features extracted using Librosa  
- **Output:** Predicted chicken sound category (e.g., *Eating*, *Happy*, *Hungry*, *Unknown*)  
- **Accuracy:** Depends on dataset quality (~85–90% on sample data)  

---

## 🏁 Future Enhancements
- 🎙️ Real-time chicken sound detection using microphone input.  
- 📱 Deploy model on a web or mobile app interface.  
- 📡 Integrate IoT sensors for farm health monitoring.  
- 🔊 Expand dataset with more diverse chicken sound categories.  

---

## 📜 License

This project is licensed under the **MIT License** — you’re free to use and modify it with attribution.

---

⭐ **If you found this project helpful, don’t forget to give it a star!**  
👉 [GitHub Repository](https://github.com/anaggha30/Chicken-Sound)
