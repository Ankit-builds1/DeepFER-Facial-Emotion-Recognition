# 🚀 DeepFER: Facial Emotion Recognition
### Deep Learning for Computer Vision

Python TensorFlow OpenCV

A real-time facial emotion recognition system trained to predict seven types of emotions: **Angry, Disgust, Fear, Happy, Neutral, Sad, and Surprise.**

---

## 📌 Project Overview
Traditional customer satisfaction surveys are often biased and lack real-time feedback. **DeepFER** leverages deep learning to automatically detect emotions. By utilizing Convolutional Neural Networks (CNNs) and Transfer Learning, the system bridges the gap between AI and empathetic human-computer interaction.

---

## 🛠️ Key Features & Techniques
* **Custom CNN Architecture**: Built from scratch utilizing Global Average Pooling (GAP) to drastically reduce overfitting.
* **Transfer Learning (ResNet50)**: Fine-tuned with heavy ImageNet weights maximizing accuracy & support for superior feature extraction.
* **Advanced Data Augmentation**: Implemented Random Rotation, Width/Height Shift, Zoom, and Random Shearing to avoid over-reliance on pixel locations.
* **Class Imbalance Handling**: Utilized computed class weights and Focal Loss to handle minor FER2013 data.
* **Test-Time Augmentation (TTA)**: Average predictions over 5 augmented views to boost accuracy.

---

## 📊 Performance Metrics

| Model Architecture | Validation Accuracy | Loss |
| :--- | :--- | :--- |
| Custom CNN Model | ~65.4% | 0.92 |
| ResNet50 Transfer Learning | ~71.8% | 0.78 |

*(Graphs for Training & Validation Curves can be viewed inside the notebooks)*

---

## 🚀 Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com
cd DeepFER-Facial-Emotion-Recognition
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the Notebook
Open `notebooks/DeepFER_Training_and_Evaluation.ipynb` in Jupyter Notebook or Kaggle, and ensure you have downloaded the FER2013 dataset.

---



---

## 🔮 Future Scope
* Real-time network integration using OpenCV.
* Deployment as a web application using Streamlit or Flask.
* Optimizing with TensorRT for faster inferencing on edge devices.
