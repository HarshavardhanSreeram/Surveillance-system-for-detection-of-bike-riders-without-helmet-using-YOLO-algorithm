# Motorcycle Helmet Detection System Using YOLOv8

This project focuses on developing a surveillance system using the YOLO (You Only Look Once) algorithm, specifically YOLO version 8, to detect motorbike riders who are not wearing helmets. The system aims to improve road safety by identifying and highlighting instances of riders without helmets, thus ensuring adherence to safety regulations.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Training](#model-training)
- [Results](#results)
- [Acknowledgments](#acknowledgments)

## Introduction

Motorcycles serve as a prevalent means of transportation in many countries. However, riding one poses significant risks without proper safety measures. This project leverages the YOLOv8 algorithm to accurately detect motorbike riders who are not wearing helmets. By utilizing an enhanced iteration of the YOLO algorithm, the model's efficiency and precision in detecting traffic violations have been significantly improved.

## Features

- Real-time detection of motorbike riders without helmets
- High accuracy and efficiency using YOLOv8
- Easy to integrate with surveillance systems
- Helps in reducing traffic incidents by ensuring adherence to safety regulations

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/helmet-detection-yolov8.git
    ```
2. Navigate to the project directory:
    ```bash
    cd helmet-detection-yolov8
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. To run the detection on a video feed:
    ```bash
    python detect.py --source video.mp4 --weights yolov8.pt
    ```
2. To run the detection on a live webcam feed:
    ```bash
    python detect.py --source 0 --weights yolov8.pt
    ```

## Dataset

The model has been trained on a custom dataset of images and videos of motorbike riders with and without helmets. The dataset includes diverse scenarios to ensure the model's robustness.

## Model Training

To train the model on your own dataset, follow these steps:

1. Prepare your dataset in the required format.
2. Modify the `train.py` script with the appropriate dataset path and other parameters.
3. Run the training script:
    ```bash
    python train.py --data dataset.yaml --weights yolov8.pt --epochs 50
    ```

## Results

The YOLOv8 model has shown significant improvements in detecting motorbike riders without helmets with high accuracy and low false positive rates. The detailed results and performance metrics can be found in the `results` directory.

## Acknowledgments

- The YOLOv8 algorithm
- Open source contributors
