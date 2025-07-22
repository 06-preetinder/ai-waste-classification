# ♻️ Waste Classification using Custom CNN

This is a deep learning project built to classify images of waste into six categories: **cardboard**, **glass**, **metal**, **paper**, **plastic**, and **trash**.  
It uses a **Convolutional Neural Network (CNN)** model built **from scratch using TensorFlow and Keras**, trained on a real-world dataset.

---

## 📁 Project Structure

```
├── notebooks/
│   └── 1_data_preprocessing.ipynb
│   └── 2_model_testing_and_visualization.ipynb
│   └── README.md 
├── saved_model/
│   └── model.md (Drive link to download model)
├── dataset/
│   └── dataset.md (Drive link to download dataset)
│   └── split_dataset.md (Drive link to download split dataset)
│   └── test_images.md (Used for real-world testing)
├── requirements.txt
└── README.md
```

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

---

## 📊 Results

| Metric         | Value      |
|----------------|------------|
| **Accuracy**   | ~77%       |
| **Loss**       | ~0.60      |
| **Real Image Testing** | ✅ Successful |

- Trained for up to 30 epochs with early stopping
- Performance evaluated on test data and real-world phone images
- Dataset was moderately imbalanced

---

## 📦 Dataset

The dataset consists of images of waste materials categorized into:

- `cardboard`
- `glass`
- `metal`
- `paper`
- `plastic`
- `trash`

---

## 🤖 Model Download

The trained model has been saved in `.h5` format using Keras.

🔗 [Download Model](https://drive.google.com/file/d/1lOMha3wCnn2NwsqzvXYHnwEMG2lH4Vtx/view?usp=sharing)

---

## 🧪 Real-World Testing

Sample test images captured from a phone were used to verify model performance.  
These images were placed in the `test_images/` folder and predictions were made using `model.predict()` after proper preprocessing.

You can test your own images by uploading them to the same folder and running the final prediction notebook.

---

## 💻 How to Run Locally

1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/waste-classification-ai.git
   cd waste-classification-ai
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the Jupyter notebook:
   ```bash
   jupyter notebook
   ```

---

## 🚀 Streamlit UI (Coming Soon)

We are working on a **Streamlit-based UI** to allow:
- 📸 Real-time prediction via webcam or image upload
- 📊 Class probability visualization
- ⚡ Fast local execution

Stay tuned!

---

## 🙌 Acknowledgments

- Dataset: [Kaggle Waste Classification Dataset](https://www.kaggle.com/datasets)
- TensorFlow + Keras for training
- Google Colab for experimentation
- GitHub for project versioning

---

## 📧 Contact

**Preetinder Singh**  
🖥️ GitHub: [06-preetinder](https://github.com/06-preetinder)  


