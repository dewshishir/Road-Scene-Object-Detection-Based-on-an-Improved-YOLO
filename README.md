Road Scene Object Detection Based on an Improved YOLO
Project Overview

This project implements a multi-class road scene object detection system using an improved YOLO-based architecture. The model is designed for dense urban traffic environments, specifically Bangladesh city traffic scenarios.

The system performs real-time detection on both images and videos, handling heavy traffic congestion, occlusion, and multi-object scenes.

Detected Object Classes

The trained model detects:

Car

Bus

CNG (Auto-rickshaw)

Motorbike

Bicycle

Pickup

MPV

Rickshaw

Shopping Van

Pedestrian

The detection results demonstrate stable confidence scores in crowded and complex intersections.

Repository Contents

The repository includes:

Traffic_using_Improved_YOLO.ipynb
Full implementation notebook (training, validation, inference)

Three real traffic video samples:

Incredible traffic jam in Dhaka, Bangladesh

Traffic Signal In Dhaka City (part-2)

Traffic jam in dhaka city.mp4

These videos are used to evaluate real-world inference performance.

Model Architecture

Base Framework: Ultralytics YOLO

Improved detection pipeline

Anchor-free detection head

Optimized NMS

Efficient backbone

Training configuration:

Input size: 640×640

Epochs: 50

Batch size: 8

Early stopping enabled

Performance Evaluation

The model is evaluated using:

mAP@50

mAP@50-95

Precision

Recall

Confusion Matrix

Per-class mAP

Validation example:

metrics = model.val(data='data.yaml')

print(metrics.box.map50)
print(metrics.box.map)
print(metrics.box.mp)
print(metrics.box.mr)
Video Inference

Inference is performed on real Dhaka traffic footage:

results = model.predict(
    source='video_path',
    save=True,
    conf=0.5
)

Output includes:

Annotated bounding boxes

Class labels

Confidence scores

Processed detection video

Key Capabilities

Dense traffic detection

Multi-object simultaneous detection

Pedestrian and vehicle separation

High congestion scene handling

Real-world Bangladesh traffic validation

Colab Notebook

Full implementation available at:

https://colab.research.google.com/drive/1VxfdNGWPOPmYGHfwjBrpGH83sB9Ee-jr?usp=sharing

Applications

Smart traffic monitoring

Traffic density estimation

Vehicle counting

Intelligent signal systems

Urban surveillance analytics

Author

Monowar Islam
BSc Computer Science and Engineering
Deep Learning and Computer Vision
