# 🎯 Real-Time Color Based Object Detection using OpenCV

## 📌 Overview
This project demonstrates how to detect and track colored objects in real time using a webcam.  
It uses **OpenCV**, **NumPy**, and **Pillow (PIL)** to perform color segmentation in the **HSV color space** and draws bounding boxes around detected objects.

The system is fast, simple, and suitable for beginners who want to understand how computer vision works at a mathematical and practical level.

---

## 🚀 Features
- Live webcam feed processing  
- HSV-based color detection  
- Noise-tolerant thresholding  
- Automatic bounding box extraction  
- Real-time visualization  
- Beginner-friendly and well-structured code  

---

## 🧠 Core Concept

### Why HSV instead of BGR/RGB?
RGB/BGR mixes color and brightness, which makes detection unreliable under different lighting conditions.  
HSV separates:

- **Hue (H)** → Type of color  
- **Saturation (S)** → Purity of color  
- **Value (V)** → Brightness  

This separation allows stable and mathematically clean color detection.

---

## 🧮 Mathematical Logic Behind Detection

This creates a **binary mask**:
- White (255) → detected color  
- Black (0) → background  

The bounding box is then computed around the cluster of white pixels.

---

## 🛠️ Technologies Used
- **Python**
- **OpenCV** – image processing and camera handling  
- **NumPy** – numerical operations and array handling  
- **Pillow (PIL)** – bounding box extraction from mask  

---

## 📂 Project Structure

---

## 🔁 How the System Works

1. Capture video from webcam  
2. Convert each frame from **BGR → HSV**  
3. Convert the reference color into HSV  
4. Generate tolerance range for Hue  
5. Apply thresholding to create a mask  
6. Find bounding box of detected pixels  
7. Draw rectangle on original frame  
8. Display results in real time  

---

## ▶️ How to Run the Project

### 1️⃣ Install dependencies
```bash
pip install opencv-python numpy pillow
python scratch.py


For every pixel in the frame:

