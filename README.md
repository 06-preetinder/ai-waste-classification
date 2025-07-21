# ♻ AI-Based Waste Classification Project

> Built with TensorFlow + EfficientNet + Google Colab  
> Predicts type of waste from image input (Plastic, Paper, Glass, etc.)

---

## 📌 Overview

This project focuses on automating the classification of waste materials using deep learning, specifically transfer learning with EfficientNet. The goal is to aid proper waste sorting for recycling and environmental management.

---

## 🧠 Model Details

- 🔍 *Architecture*: EfficientNetB0 (Transfer Learning)
- 📈 *Training Accuracy*: ~78(apx)%
- 🧪 *Test Accuracy*: ~60(apx)%
- 🧩 *Classes*: cardboard, glass, metal, paper, plastic

---

## 🗂 Project Structure
waste-classification-ai/
├── notebooks/
│ ├── 1_data_preprocessing_and_training.ipynb
│ └── 2_model_evaluation_and_testing.ipynb
├── test_images/ # Real-world images tested
├── saved_model/ # Google Drive link
├── dataset/ # Google Drive link
├── requirements.txt
└── README.md
---

## 🧪 Sample Predictions

| Image | Prediction |
|-------|------------|
| ![](test_images/plastic1.jpg) | `Plastic` |
| ![](test_images/paper1.jpg)   | `Paper`   |

---

## 📁 Dataset & Model

> Due to size limits, the dataset and trained model are stored in Google Drive.

- 📦 [Download Dataset (Split into Train/Val/Test)](https://drive.google.com/your_dataset_link)
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
