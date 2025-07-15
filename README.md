# 🎓 Signal & Video Processing Experiments

This document summarizes two core experiments performed using Python for media signal analysis:  
- **Experiment 1**: Human Activity Recognition in Video  
- **Experiment 2**: Audio Signal Analysis using Librosa

---

## 🧪 Experiment 1: Human Activity Recognition in Video

This experiment uses **MediaPipe** and **OpenCV** to detect human poses in video frames and visualize body landmarks in real time.

### 🔍 Objective
To detect human activities like walking, standing, etc., by identifying key body joints using pre-trained pose estimation models.

### 🛠️ Tools & Libraries
- **OpenCV** – For reading and displaying video
- **MediaPipe** – For human pose estimation
- **Python** – Language for implementing real-time inference

### ⚙️ Workflow
1. Load a pre-recorded video file using `cv2.VideoCapture`.
2. Convert each frame from BGR to RGB (required by MediaPipe).
3. Use `mp.solutions.pose` to process each frame and detect body landmarks.
4. Overlay pose landmarks and skeletal connections on the original frame.
5. Display live video with pose tracking until the video ends or user exits.

### 📈 Output
A real-time video window showing:
- Pose landmarks (e.g., elbows, knees)
- Skeleton connections between body joints

### 📌 Applications
- Fitness and yoga tracking
- Motion capture in sports
- Gesture recognition and body language detection

---

## 🎧 Experiment 2: Audio Signal Analysis using Librosa

This experiment involves analyzing a `.wav` audio file using various signal processing techniques to extract time, frequency, and energy-related information.

### 🔍 Objective
To understand the structure and characteristics of an audio signal by visualizing:
- Waveform
- Spectrogram
- Energy levels
- Fundamental frequency (Pitch)

### 🛠️ Tools & Libraries
- **Librosa** – For audio signal processing
- **Matplotlib** – For visualizing signal properties
- **NumPy** – For numerical operations
- **Python** – Primary scripting language

### ⚙️ Workflow
1. Load the audio file using `librosa.load()`.
2. Display waveform in time-domain.
3. Compute Short-Time Fourier Transform (STFT) and plot the spectrogram.
4. Calculate short-time energy using frame-based sliding window.
5. Extract pitch (F0) using `librosa.pyin()`.

### 📈 Output Visuals
| Visualization         | Description                                       |
|------------------------|---------------------------------------------------|
| **Waveform**           | Amplitude vs Time                                 |
| **Spectrogram**        | Frequency vs Time (in decibels)                   |
| **Short-Time Energy**  | Temporal energy variation                         |
| **Pitch Estimation**   | Extracted pitch contour across time               |

### 📌 Applications
- Speech recognition
- Music genre classification
- Emotion detection in speech
- Speaker verification
- Onset detection in music

---

## ✅ Summary

| Experiment | Techniques Used                   | Tools                      | Output |
|------------|-----------------------------------|----------------------------|--------|
| Human Activity Recognition | Pose Estimation (MediaPipe)       | OpenCV, MediaPipe           | Live annotated video |
| Audio Analysis            | STFT, Energy, F0 Extraction       | Librosa, Matplotlib, NumPy | Waveform, Spectrogram, Pitch graph |

---

> These experiments form a foundational understanding of how machines can interpret and analyze both **visual motion** and **acoustic signals** for real-world intelligent applications.

