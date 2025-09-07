# sign-language-recognition
Custom Sign Language Recognition system using a self-built dataset and a deep learning model (Keras + OpenCV + cvzone) to translate hand gestures into real-time alphabet predictions.

# 🖐️ Sign Language Recognition using Custom Dataset and Deep Learning

## 📑 Project Overview
This project implements a **real-time Sign Language Recognition system** that translates hand gestures into alphabet predictions.  
We built a **custom dataset** of hand gestures, trained a **CNN model (Keras/TensorFlow)**, and used **OpenCV + cvzone** for hand detection and live classification.  

The goal is to **bridge communication gaps** between sign language users and non-signers by enabling fast, accurate, and accessible sign recognition.

---

## 🔬 Features
- ✅ Built on a **custom dataset** of static sign language gestures.  
- ✅ **CNN-based model** trained with TensorFlow/Keras.  
- ✅ Real-time hand detection using **cvzone.HandDetector**.  
- ✅ Gesture classification for **A–Z alphabets** (excluding dynamic signs J & Z).  
- ✅ Modular code for easy extension to other datasets (ASL, ISL, etc.).  

---

## 📂 Dataset
We created a **custom dataset** consisting of labeled hand gesture images for alphabets.  
The preprocessing pipeline ensures consistency by resizing and centering hand images to `300x300` pixels on a white background.  

Other datasets that can be integrated:  
- RWTH-BOSTON-104  
- ASL Lexicon Video Dataset  
- Sign Language MNIST  
- Indian Sign Language Dataset  

---

## 🧠 Model
- **Architecture**: Convolutional Neural Network (CNN)  
- **Frameworks**: TensorFlow / Keras  
- **Trained model file**: `Model/Hand_Model.h5`  
- **Labels file**: `Model/Labels.txt`  

The model was trained with image augmentation and achieves high accuracy on the custom dataset.

---

## 💻 How to Run
### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/sign-language-recognition.git
cd sign-language-recognition
