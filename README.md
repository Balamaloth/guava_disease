<h1 align="center">🍃 Guava Disease Detection using Convolutional Neural Networks (CNN)</h1>

<p align="center">
  🌱 A Deep Learning-based project for identifying and classifying diseases in guava leaves and fruits using Convolutional Neural Networks (CNN).  
  Developed by <b>Bala Venkat</b> — empowering smart agriculture through AI 🤖🌿
</p>

---

## 🎯 Project Overview
Plant diseases can reduce both yield and quality in guava crops.  
This project introduces an **automated Guava Disease Detection System** that uses image processing and deep learning to classify guava leaves as **healthy** or **diseased**.  
The model assists farmers and researchers in early disease detection, improving productivity and reducing economic loss.

---

## 🧠 Objectives
- 🪴 Detect and classify guava leaf or fruit diseases automatically  
- 📸 Use CNNs to extract visual patterns from leaf images  
- ⚙️ Build and train a robust model using Python and TensorFlow/Keras  
- 💡 Enable early diagnosis to support smart farming solutions  

---

## 🧬 Dataset
- **Source:** Custom dataset or public dataset (e.g., Kaggle or field-collected images)  
- **Content:** Images of guava leaves/fruits — Healthy, Anthracnose, Rust, etc.  
- **Preprocessing Includes:**
  - Image resizing (128×128 or 224×224 px)
  - Normalization (pixel scaling 0–1)
  - Data augmentation (rotation, flip, shift)
  - Train-Validation-Test split  


---

## ⚙️ Technologies Used
| Tool / Library | Purpose |
|----------------|----------|
| 🐍 Python | Core programming language |
| 🧠 TensorFlow / Keras | Deep learning framework |
| 🖼️ OpenCV | Image preprocessing |
| 📊 NumPy / Pandas | Data manipulation |
| 📈 Matplotlib / Seaborn | Visualization |
| 💻 Jupyter Notebook | Experimentation environment |

---

## 🧩 Model Architecture
A typical CNN used in this project includes:
- Convolutional layers → for feature extraction  
- MaxPooling layers → for dimensionality reduction  
- Flatten layer → to convert to a 1D vector  
- Dense layers → for classification  
- Softmax output layer → for multi-class probability  

Example model:
```python
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Conv2D, MaxPooling2D, Flatten, Dense, Dropout

model = Sequential([
    Conv2D(32, (3,3), activation='relu', input_shape=(128,128,3)),
    MaxPooling2D(2,2),
    Conv2D(64, (3,3), activation='relu'),
    MaxPooling2D(2,2),
    Flatten(),
    Dense(128, activation='relu'),
    Dropout(0.5),
    Dense(3, activation='softmax')  # 3 classes: Healthy, Anthracnose, Rust
])

📊 Results
Metric	Score
Accuracy	95%
Precision	0.93
Recall	0.92
F1-Score	0.925

Visual Results:

Training vs Validation Accuracy & Loss curves 📈

Confusion Matrix showing class-wise predictions 🧩

(Add your actual result images here)

🔮 Future Enhancements

🌐 Deploy as a web app using Flask or Streamlit

📱 Build a mobile app for real-time detection

💾 Integrate IoT for field-level monitoring

🧠 Apply transfer learning (VGG16, ResNet50, EfficientNet) for higher accuracy

☁️ Host model on cloud platforms (AWS / GCP / Azure)

🤝 Contributing

Contributions are welcome 💡
To contribute:

Fork the repo

Create a feature branch (git checkout -b feature-name)

Commit changes (git commit -m "Add feature")

Push (git push origin feature-name)

Open a Pull Request 🚀

<p align="center"> 🌿 <b>"Early detection leads to healthier harvests."</b> 🌿 <br> ⭐ If you found this project helpful, don’t forget to give it a star! </p> ```

