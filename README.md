# 👁️‍🗨️ Face Recognition Attendance System (FRAS)

This project presents **FRAS**, an AI-powered face recognition attendance system developed to automate and improve attendance management in educational settings.

## 📌 Project Overview

FRAS uses **FaceNet** for face embedding extraction and a **Support Vector Machine (SVM)** classifier to identify students from classroom images. The system allows teachers to take attendance by simply capturing a photo of the class.

> ✅ Key Benefits:
- Saves time by eliminating manual attendance
- Reduces human error
- Provides real-time reports
- Scales with classroom size and student growth

---

## 🧠 Technologies Used

- **Python**
- **FaceNet** (for 128-d face embeddings)
- **MTCNN** (for face detection)
- **SVM** (for classification)
- **OpenCV**
- **Keras**
- **scikit-learn**

---

## 🗂 Dataset & Preprocessing

- Collected face images per student, labeled by name and ID
- Applied **data augmentation**: rotation, translation, zoom, flipping, brightness
- Used FaceNet to convert images into embeddings
- Trained SVM classifier on the embeddings

---

## ⚙️ System Workflow

1. Detect faces in a classroom image using MTCNN
2. Crop and resize each detected face (160×160 px)
3. Extract facial embeddings using FaceNet
4. Classify embeddings using SVM to identify students
5. Record attendance in a database or Excel file

---

## 📈 Results

- Achieved **99% accuracy**
- High precision, recall, and F1-score across test cases
- Robust to lighting, expressions, and partial occlusions
- Tested on large datasets without performance loss

---

## 🧩 Features

- Real-time attendance marking
- Handles partial occlusions and diverse expressions
- User-friendly interface for teachers
- Secure data handling and storage

---

## 📚 Future Work

- Integrate with school management systems
- Expand to multimodal authentication (e.g., voice, fingerprint)
- Cloud-based deployment with mobile app support

---

## 👨‍💻 Authors

- Jawad
- Abdulaziz
- Khaled
- Mohammed
- Faisal  
