# Fall Detection using MediaPipe Pose Estimation

This project implements a real-time human fall detection system using **MediaPipe's Pose Landmarks** model. It is designed for use in industrial environments to help detect unconscious or fallen workers and alert supervisors immediately.

---

## 📌 Features

- Detects full-body human pose in real time using a webcam
- Identifies potential falls or abnormal postures using landmark positions
- Overlays visual pose skeleton on the video feed for monitoring
- Useful in factories, warehouses, construction sites, and healthcare settings
- Lightweight enough for deployment on laptops or embedded devices

---

## 🧠 Methodology

- Utilizes **MediaPipe Pose** to track 33 human body landmarks
- Continuously monitors the user's pose and posture
- Detects sudden posture shifts or floor-level body orientation that may indicate a fall
- Visual overlay rendered using OpenCV to assist with manual monitoring or debugging

---

## 🎯 Detection Logic (Conceptual)

- **Key Landmark Ratios**: Tracks the position of hips, shoulders, and head relative to each other and the floor
- **Torso Angle**: Computes the inclination of the torso to detect slumped or collapsed positions
- **Velocity of Change**: Optionally integrates future support for abrupt pose changes
- **Fall Indication**: Triggered when the lower body is unnaturally aligned or flat on the ground

---

## 🖼️ Visual Output

- Full-body landmark skeleton rendered on live video stream
- Color-coded connections to indicate tracked joints
- Window shows real-time updates

---

## ⚙️ System Requirements

- Python 3.7+
- Webcam or external camera
- Basic desktop or laptop GPU (NVIDIA optional)
- MediaPipe library for pose estimation
- OpenCV for video streaming and drawing overlays

---

## 📦 Dependencies

- `mediapipe`
- `opencv-python`
- `numpy`


