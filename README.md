# Football Players Tracking and Detecting Collision Risk ⚽

## Overview ✨
This project aims to track football players' movement using **YOLOv8** and **DeepSORT**. It processes a Kaggle-based football image dataset to detect and track players, calculate their velocities, and identify potential collisions during a match.

---

## Dataset 📁
- Images of football matches from Kaggle
- Annotations are converted to YOLOv8-compatible format
- Focused only on **players**

---

## Key Features 🔧

### 1. Preprocessing ⚙️
- Converts dataset to YOLO format
- Performs exploratory data analysis (EDA) including:
  - Number of images and annotations
  - Class distribution (filtering for "person")
  - Sample visualization of images and masks
- Augmentation avoids flips and shifts to maintain spatial accuracy

### 2. Fine-Tuning YOLOv8 🧠
- YOLOv8 is fine-tuned on the custom dataset for improved player detection

### 3. DeepSORT Tracking 🛰️
- Tracks players across frames using DeepSORT
- Calculates player velocities from positional differences

### 4. Collision Prediction 🚨 
- Uses player speed and direction to predict possible collisions

### 5. Video Inference 🎥
- Applies the model to input football videos
- Displays bounding boxes, player ID, speed, and collision risk

---

## Visualization & Reports 📊
- Plots and summaries of player statistics
- Exports visual reports as PDF

---

## Dependencies 🛠️ 
The notebook installs required packages including:
- `ultralytics`
- `opencv-python`
- `numpy`, `pandas`, `matplotlib`
- `torch`, `torchvision`


---

## 👩‍💻 Supervised by 
- Noor Felemban

## 👥 Authors
- Shahad Adel
- Deem Alrashidi
- Sahar Alshehri
- Sara Thaer
- Sana Araj
