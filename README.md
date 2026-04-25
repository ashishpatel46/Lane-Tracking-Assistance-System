# Lane Detection Using OpenCV (Python)

This project implements a **lane detection system** using classical **computer vision techniques**.  
It processes a road video frame by frame, detects lane lines, and draws them on the output video.

The project is inspired by **autonomous driving systems**, where lane detection plays an important role in vehicle navigation.

---

## Features
- Detects **left and right lane lines** from road videos
- Uses **Canny Edge Detection** for edge extraction
- Applies **Region of Interest (ROI)** to focus only on the road
- Uses **Hough Line Transform** to detect straight lane lines
- Draws smooth and stable lane lines on video frames
- Supports **step-by-step visualization** for debugging

---

## Technologies Used
- Python  
- OpenCV  
- NumPy  
- MoviePy  
- Google Colab  

---

## Methodology

1. Convert each video frame to **grayscale**
2. Apply **Gaussian Blur** to reduce noise
3. Detect edges using **Canny Edge Detection**
4. Mask unnecessary regions using **Region of Interest**
5. Detect line segments using **Hough Line Transform**
6. Separate left and right lanes using slope calculation
7. Average detected lines for stability
8. Draw final lane lines on the original frame

---

## 📂 Project Structure
```bash
Lane-Detection/
│
├── test2.mp4 # Input road video
├── output.mp4 # Output video with lane detection
├── lane_detection.ipynb
└── README.md
```

---

## ▶️ How to Run

1. Clone the repository
```bash
git clone https://github.com/Mohitpr1314/lane-detection-opencv.git

```

2. Install required libraries
```bash
pip install opencv-python numpy moviepy
```

3. Place your input video as input.mp4
4. Run the script
```bash
python lane_detection.py

```
5. The output will be saved as output.mp4



