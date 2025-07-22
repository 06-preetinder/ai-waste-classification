# ♻ AI-Based Waste Classification Project

> Built with TensorFlow | Custom Scratch CNN | Trained in Google Colab

> Predicts type of waste from image input (Plastic, Paper, Glass, etc.)


---

## 📌 Overview

This project focuses on automating the classification of waste materials using deep learning, specifically a custom Convolutional Neural Network (CNN) built from scratch.The goal is to aid proper waste sorting for recycling and environmental management using image-based classification.

---

## 🧠 Model Architecture

A simple yet effective **scratch-built CNN** was trained using the Keras `Sequential` API.

```python
model = Sequential([
    Conv2D(32, (3,3), activation='relu', input_shape=(224, 224, 3)),
    MaxPooling2D(2,2),
    Conv2D(64, (3,3), activation='relu'),
    MaxPooling2D(2,2),
    Flatten(),
    Dense(128, activation='relu'),
    Dense(6, activation='softmax')
])
```
- 📈 *Training Accuracy*: ~78(apx)%
- 🧪 *Test Accuracy*: ~60(apx)%
- 🧩 *Classes*: cardboard, glass, metal, paper, plastic

---

## 📁 Project Structure

```
├── notebooks/
│   └── 1_data_preprocessing_and_training.ipynb
├── saved_model/
│   └── README.md (Drive link to download model)
├── dataset/
│   └── README.md (Drive link to download dataset)
├── test_images/
│   └── README.md (Used for real-world testing)
├── requirements.txt
└── README.md
```

---

## 🧪 Sample Predictions

| Image | Prediction |
|-------|------------|
| ![view](https://drive.google.com/file/d/1oI-3UcxSTm0gAVSOA17VmqzfXRTuYgdj/view?usp=drive_link) | `Metal` |
| ![view](https://drive.google.com/file/d/13HXWpD51nfLlWk7LIVPj95HUrWMT9aj7/view?usp=drive_link)   | `Paper`   |

---

## 📁 Dataset & Model

> Due to size limits, the dataset and trained model are stored in Google Drive.

- 📦 [Download Dataset (Split into Train/Val/Test)](https://drive.google.com/drive/folders/1oIywZck3iC9zEzr6K2tUmmNUxv_U_uXi?usp=drive_link)
- 🤖 [Download Trained Model (.h5)](https://drive.google.com/file/d/1lOMha3wCnn2NwsqzvXYHnwEMG2lH4Vtx/view?usp=drive_link)

---

## ⚙️ How to Run Locally

1. Clone the repository:
    ```bash
    git clone https://github.com/06-preetinder/ai-waste-classification.git
    ```

2. Open notebooks in Google Colab or VSCode/Jupyter

3. Install dependencies (optional):
    ```bash
    pip install -r requirements.txt
    ```

---

## 🧪 Real-World Testing

We tested the model on real images from mobile camera and verified performance. You can add your own images in `test_images/` and test using notebook #2.

---

## 💡 Future Work

- 🌐 Streamlit-based UI (real-time webcam input)
- ☁️ Deploy to HuggingFace or Render
- 📊 Improve model accuracy using more balanced data

---

## 🙌 Credits

- Built by: PreetinderjeetSingh
- July 2025

---

## 🛠️ Requirements
tensorflow
numpy
matplotlib
pandas
seaborn
scikit-learn
split-folders
