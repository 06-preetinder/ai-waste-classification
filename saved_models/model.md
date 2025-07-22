🧠 Model Architecture
This project uses a Convolutional Neural Network (CNN) built from scratch using TensorFlow and Keras. The model was trained to classify waste into six categories: cardboard, glass, metal, paper, plastic, and trash.

🧩 Architecture:
python
Copy
Edit
model = Sequential([
    Conv2D(32, (3,3), activation='relu', input_shape=(224, 224, 3)),
    MaxPooling2D(2,2),
    Conv2D(64, (3,3), activation='relu'),
    MaxPooling2D(2,2),
    Flatten(),
    Dense(128, activation='relu'),
    Dense(6, activation='softmax')
])
✅ Model Highlights:
Built from scratch without pre-trained weights

Lightweight and fast to train — ideal for basic systems or beginner projects

Trained on a real-world waste classification dataset (~2,500+ images)

📈 Performance:
Training Accuracy: ~77%

Training Loss: ~0.60

Tested on real-world images captured via phone camera

Accuracy may vary depending on class imbalance and image noise

🔗 Download the trained model (.h5) from Google Drive:

[Download Model](https://drive.google.com/file/d/1lOMha3wCnn2NwsqzvXYHnwEMG2lH4Vtx/view?usp=sharing)
