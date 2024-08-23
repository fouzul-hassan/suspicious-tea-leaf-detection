# YOLOv8 Streamlit Interface


YOLOv8 Streamlit Interface is a user-friendly web app for real-time object detection using YOLOv8. Built with Streamlit, it supports various YOLOv8 models and multiple input types, including images, videos, and webcam streams. This tool is perfect for researchers and developers who want an easy way to experiment with state-of-the-art object detection technology.


## Introduction

Welcome to the YOLOv8 Streamlit App! This project provides a user-friendly, interactive interface for [YOLOv8](https://github.com/ultralytics/ultralytics) object detection using [Streamlit](https://github.com/streamlit/streamlit). This tool is ideal for researchers, developers, and hobbyists looking to experiment with object detection models in a simplified manner.

## Features

- **Object Detection**: Perform real-time object detection tasks using state-of-the-art YOLOv8 models.
- **Multiple Detection Models**: Easily switch between different YOLOv8 model sizes:
  - `yolov8n` (Nano)
  - `yolov8s` (Small)
  - `yolov8m` (Medium)
  - `yolov8l` (Large)
  - `yolov8x` (Extra Large)
- **Multiple Input Formats**: Supports detection on various inputs:
  - `Image` files
  - `Video` files
  - `Webcam` for live detection

## Installation

### Prerequisites

- [Anaconda](https://www.anaconda.com/products/distribution) installed on your system.
- Basic knowledge of Python and command-line tools.

### 1. Create a New Conda Environment

First, create and activate a conda environment named `yolov8-streamlit`:

```bash
# Create a new environment
conda create -n yolov8-streamlit python=3.8 -y

# Activate the environment
conda activate yolov8-streamlit
```

### 2. Clone the repo

```bash
git clone https://github.com/fouzul-hassan/yolov8-streamlit-interface
cd yolov8-streamlit-interface

```


### 3. Install packages
```commandline
# yolov8 dependencies
pip install ultralytics

# Streamlit dependencies
pip install streamlit
```
### 4. Download Pre-trained YOLOv8 Detection Weights
Create a directory named `weights` and create a subdirectory named `detection` and save the downloaded YOLOv8 object detection weights inside this directory. The weight files can be downloaded from the table below.

| Model                                                                                | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
| ------------------------------------------------------------------------------------ | --------------------- | -------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt) | 640                   | 37.3                 | 80.4                           | 0.99                                | 3.2                | 8.7               |
| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640                   | 44.9                 | 128.4                          | 1.20                                | 11.2               | 28.6              |
| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt) | 640                   | 50.2                 | 234.7                          | 1.83                                | 25.9               | 78.9              |
| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l.pt) | 640                   | 52.9                 | 375.2                          | 2.39                                | 43.7               | 165.2             |
| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt) | 640                   | 53.9                 | 479.1                          | 3.53                                | 68.2               | 257.8             |


### 5. Running the application
```commandline
streamlit run app.py
```
Then will start the Streamlit server and open your web browser to the default Streamlit page automatically.


***

If you also like this project, you may wish to give a `star` (^.^)✨ . If any questions, please raise `issue`~
