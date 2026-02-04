# 🎾 Tennis Match Analysis using Computer Vision

## Introduction

This project performs **automated tennis match analysis from video footage** using computer vision and deep learning techniques. It detects and tracks players and the tennis ball, identifies ball hit events, and visualizes gameplay using a **mini-court overlay**, enabling structured and meaningful analysis from raw match videos.

The system leverages **YOLO-based object detection** for players and the ball, along with **CNN-based court keypoint extraction**, to understand both motion and spatial context. This hands-on, end-to-end project is ideal for strengthening skills in **machine learning, computer vision, and video analytics**.

---

## 🎥 Output Videos

The final output video includes:
- Player bounding boxes with unique IDs  
- Tennis ball tracking  
- Court keypoints  
- Mini-court visualization
- Ball hit detection
- Speed of shots
- Speed of players  

📸 *Example output frame:*  
<img width="960" height="544" alt="{260F99C7-F838-4F88-BD40-0D6C88852EE0}" src="https://github.com/user-attachments/assets/fd397c50-8f71-4d1c-b34d-4230a6de52b4" />

---

## 🧠 Models Used

- **YOLOv8** – Player detection  
- **Fine-tuned YOLOv5** – Tennis ball detection  
- **CNN-based (ResNet50) Court Keypoint Detection** – Court geometry extraction  

### Pretrained / Trained Models

- 🎾 **Tennis Ball Detection Model (YOLOv5)**  
  https://drive.google.com/file/d/1UZwiG1jkWgce9lNhxJ2L0NVjX1vGM05U/view?usp=sharing

- 🏟️ **Tennis Court Keypoint Detection Model**  
  https://drive.google.com/file/d/1QrTOF1ToQ4plsSZbkBs3zOLkVt3MBlta/view?usp=sharing
---

## 📦 Datasets

This project uses the following datasets:

- 🎾 **Tennis Ball Detection Dataset**  
  https://universe.roboflow.com/viren-dhanwani/tennis-ball-detection

- 🏟️ **Tennis Court Keypoint Detection Dataset**  
  Dataset used for training the tennis court keypoint extraction model.  
  Download link:  
  https://drive.google.com/uc?id=1lhAaeQCmk2y440PmagA0KmIVBIysVMwu
---

## 🏋️ Training

Training notebooks are included for reproducibility and experimentation:

- **Tennis Ball Detector (YOLO)**  
  `training/tennis_ball_detector_training.ipynb`

- **Tennis Court Keypoint Detector (PyTorch)**  
  `training/tennis_court_keypoint_training.ipynb`

---

## 🛠️ Requirements

- Python **3.8+**
- `ultralytics`
- `torch` / `torchvision`
- `pandas`
- `numpy`
- `opencv-python`
