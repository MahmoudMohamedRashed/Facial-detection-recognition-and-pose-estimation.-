# Facial Detection, Recognition & Pose Estimation

A computer-vision project that performs **face detection**, **face recognition** (identification/verification), and **head-pose estimation**.  
This repository demonstrates an end-to-end pipeline: detect faces in images/video, recognize known identities, and estimate head pose (pitch, yaw, roll) for each detected face.

---

## Features

- 🔍 **Face Detection** — Fast and robust detection using classical (Haar / HOG) or modern detectors (DNN, YOLO, RetinaFace, MediaPipe).  
- 👤 **Face Recognition** — Extracts face embeddings and performs identification/verification against a local database of known faces.  
- 🎯 **Head-Pose Estimation** — Estimates pitch, yaw, and roll angles for each detected face (using solvePnP, landmark-based regression, or neural models).  
- 🎥 **Video & Camera Support** — Works with images, video files, or live camera streams.  
- 💾 **Persistence** — Optional local storage for known face embeddings (file or lightweight DB).

---

## Requirements

> Adjust depending on whether your implementation is in **Python** or **C++**.

### Python (recommended)
- Python 3.8+  
- OpenCV (`opencv-python`)  
- NumPy  
- dlib (optional, for 68-landmark) or `mediapipe` (lightweight landmarks)  
- `face_recognition` (optional, for quick embedding/recognition) or a deep model (e.g., `insightface`, `facenet-pytorch`)  
- [Optional] PyTorch or TensorFlow if using deep models.

Example install (minimal):
```bash
python -m venv venv
source venv/bin/activate         # Linux/macOS
venv\Scripts\activate            # Windows

pip install opencv-python numpy
# optional:
pip install dlib face_recognition mediapipe torch torchvision
