# Driver-Drowsiness-System-
## Overview
This project is designed to detect drowsiness in drivers using computer vision techniques. By monitoring the eye aspect ratio (EAR) in real-time, the system identifies signs of drowsiness and triggers an alert to prevent accidents.

## Features
Real-Time Eye Monitoring: Tracks the driver’s eye movement to calculate the Eye Aspect Ratio (EAR).
Drowsiness Detection: Alerts the driver when drowsiness is detected by playing an alarm sound.
OpenCV & Dlib Integration: Utilizes OpenCV for image processing and Dlib for facial landmark detection.

## Installation
1. Clone the repository: git clone https://github.com/avanya02/driver-drowsiness-detection.git
cd driver-drowsiness-detection
2. Install required libraries: pip install -r requirements.txt
3. Download the required Dlib model: Download shape_predictor_68_face_landmarks.dat
4. Extract and place it in the project directory.
5. Run the script: python driver_drowsiness_detection.py

## Usage
Camera Setup: Ensure your camera is connected or adjust the cv2.VideoCapture() source to match your camera.
Threshold Adjustment: You can adjust the thresh and frame_check values to make the detection more or less sensitive.
Alerts: When drowsiness is detected, an alert message is displayed on the screen, and an alarm sound is played.

## How It Works
The system captures frames from the webcam and converts them to grayscale.
It detects faces in the frame and identifies facial landmarks.
The Eye Aspect Ratio (EAR) is calculated for both eyes.
If the EAR falls below a specified threshold for a set number of frames, an alert is triggered.

