# 🎯 1: Human Activity Recognition in Video

This experiment demonstrates the implementation of a basic **human activity recognition system** using **MediaPipe Pose Estimation** and **OpenCV**. The goal is to detect and track human body landmarks in a prerecorded video, which visually outlines the human skeleton in motion.

---

## 🧪 Objective

To identify and draw the skeletal structure of a human performing an action (like walking) from a video input, thereby recognizing human pose and movement patterns.

---

## 🛠️ Tools & Technologies

- **Python 3.7+**
- **OpenCV** – For video capture, processing, and display.
- **MediaPipe** – For real-time pose estimation and landmark detection.
- **Walk_2.mp4** – Input video file showing a human walking.

---

## 📋 Workflow

1. Load a video file containing human activity.
2. Convert each video frame from BGR to RGB for MediaPipe compatibility.
3. Apply the MediaPipe Pose model to detect 33 human body landmarks.
4. Draw pose connections and landmarks on each frame.
5. Display the processed video in real-time.
6. Exit the visualization by pressing the `q` key.

---

## 🎥 Output

- Real-time visualization of the input video with the human pose skeleton overlaid.
- Body parts like shoulders, elbows, knees, and ankles are connected to form a pose graph.
- The system continuously updates the pose as the video progresses.

---

## 📌 Applications

- Human activity recognition (walking, running, sitting)
- Gesture-based user interfaces
- Sports and fitness analytics
- Surveillance systems
- Animation and motion tracking

---

## ⚠️ Notes

- Ensure the `Walk_2.mp4` video file is available in the project directory.
- The accuracy of pose detection depends on lighting, clarity, and visibility of the subject.
- MediaPipe Pose works best with full-body visibility and upright poses.

---
