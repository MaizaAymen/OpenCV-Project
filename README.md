# Real-Time Object Detection using OpenCV

## Project Overview

This project implements a real-time object detection system using OpenCV, leveraging a pre-trained deep learning model known as SSD MobileNet v3. The application captures live video from the webcam and detects objects in real-time, providing a visual output with bounding boxes and labels for each detected object.

## Features

- **Live Video Capture:** Captures video input from the webcam using OpenCV.
- **Pre-trained Model Loading:** Uses SSD MobileNet v3 for efficient and accurate object detection.
  - Weights: `files/frozen_inference_graph.pb`
  - Configuration: `files/ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt`
- **Class Name Handling:** Loads object labels from `files/thing.names` to provide understandable output.
- **Image Preprocessing:** Resizes, normalizes, and converts images to meet DNN requirements.
- **Detection Loop:** Continuously captures frames and detects objects with a configurable confidence threshold.
- **Visualization:** Draws bounding boxes and overlays class names on detected objects for easy identification.
- **Graceful Exit:** The application can be terminated by pressing the 'q' key, ensuring proper resource management.

## Use Cases

This project is applicable in various domains, including but not limited to:

- Real-time surveillance and monitoring systems
- Robotics applications with object avoidance
- Smart home systems with microcontrollers like Raspberry Pi
- Video analysis in research and development settings

## Prerequisites

Before running the project, ensure you have the following installed:

- Python 3.x
- OpenCV library (install with `pip install opencv-python`)

