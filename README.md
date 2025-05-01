![Example Image](<img width="869" alt="Screenshot 1446-11-03 at 9 15 36 AM" src="https://github.com/user-attachments/assets/0164994c-c24e-473c-9600-9574a8e69163" />
)

# 👁️‍🗨️ Face Recognition Attendance System (FRAS)

The Face Recognition Attendance System (FRAS) is an innovative solution designed to streamline and modernize the way attendance is recorded in educational institutions. By leveraging the power of artificial intelligence and facial recognition technologies, this project aims to automate the entire process of attendance tracking, thus replacing traditional manual methods that are often time-consuming, error-prone, and inefficient.

## 📌 Project Overview

FRAS integrates advanced computer vision and machine learning techniques to identify students from a single classroom image captured by the instructor. Specifically, it utilizes the FaceNet model for converting facial images into mathematical embeddings and employs a Support Vector Machine (SVM) classifier to accurately match these embeddings with registered student identities. This system has been carefully developed to ensure that attendance can be marked effortlessly, even in large classroom settings, with minimal user input and high reliability.

> ✅ Key Benefits:
- Significantly reduces the time required to take attendance during lectures or training sessions.
- Minimizes human errors and discrepancies typically associated with manual methods.
- Generates real-time reports and maintains an accurate attendance log that can be easily reviewed and audited.
- Designed to scale with increasing class sizes and adaptable to various educational or corporate settings.

---

## 🧠 Technologies Used

To implement this system, we relied on a robust set of tools and frameworks that are well-suited for deep learning and image processing tasks:
- **Python** as the primary programming language.
- **FaceNet** for generating high-precision 128-dimensional face embeddings.
- **MTCNN (Multi-task Cascaded Convolutional Networks)** for real-time face detection and alignment.
- **SVM (Support Vector Machine)** for identity classification.
- **OpenCV** for image manipulation and visualization.
- **Keras** and **scikit-learn** for model training, validation, and deployment.

---

## 🗂 Dataset & Preprocessing

A custom dataset was created by collecting facial images of enrolled students from various angles and expressions to ensure robustness. Each image was labeled with the student’s name and ID and subjected to an extensive preprocessing pipeline to improve model performance. This pipeline included:
- **Data Augmentation** techniques such as random rotation, scaling, translation, brightness adjustment, and flipping, which simulate real-world variations in appearance and lighting conditions.

![Data Augmentation](images/data_augmentation.png)
![MTCNN Cropped Face](images/mtcnn_cropped_face.png)

These enhancements were critical in making the model generalize better and recognize faces accurately even under non-ideal circumstances.

---

## ⚙️ System Workflow

The system follows a sequential and automated workflow:
1. Classroom images are captured and processed using MTCNN to detect all visible faces.
2. Detected faces are cropped and resized to a standard input size (160×160 pixels).
3. Each face is passed through the FaceNet model to extract a unique 128-dimensional embedding.
4. These embeddings are then classified by the pre-trained SVM model to determine the student’s identity.
5. Attendance is automatically marked in a database or exported to an Excel sheet.

---

## 📈 Results

The system demonstrated outstanding accuracy and performance in real-world test environments. Our evaluation showed that:
- FRAS achieved an overall recognition accuracy of **99%**.
- Metrics such as precision, recall, and F1-score were consistently high across all student classes.
- The system handled complex scenarios involving varied facial expressions, partial occlusions, and lighting changes with remarkable robustness.

![Class Results](images/class_results.png)
![Confusion Matrix](images/confusion_matrix.png)
![Test Results](images/test_results.png)

This level of performance makes the system a viable solution for practical deployment in schools, universities, and potentially even corporate settings.

---

## 🧩 Features

- Fully automatic attendance marking from a single image.
- Operates effectively in classrooms with challenging lighting and spatial configurations.
- User-friendly graphical interface designed for both instructors and administrative staff.
- Built-in data security protocols to ensure privacy and controlled access to attendance records.


---

## 👨‍💻 Authors
- Jawad  
- Abdulaziz 
- Khaled  
- Mohammed  
- Faisal  


