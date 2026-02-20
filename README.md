<h1 align="center">Road Scene Object Detection Based on an Improved YOLO</h1>

<p align="center">
  <b>Multi-Class Traffic Object Detection in Dense Urban Environments</b><br>
  Real-World Dhaka Traffic | Deep Learning | Computer Vision
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue">
  <img src="https://img.shields.io/badge/YOLO-Object%20Detection-green">
  <img src="https://img.shields.io/badge/Deep%20Learning-Computer%20Vision-red">
  <img src="https://img.shields.io/badge/Status-Completed-success">
</p>

<hr>

<h2>Project Overview</h2>

This project presents a <b>robust multi-class road scene object detection system</b> built using an improved YOLO-based architecture.  
The model is optimized for <b>dense, high-occlusion urban traffic environments</b>, specifically real-world Dhaka city traffic scenarios.

The system performs reliable detection in:

<ul>
<li>Heavy traffic congestion</li>
<li>Multi-lane intersections</li>
<li>Pedestrian-dense crosswalk zones</li>
<li>Mixed vehicle environments</li>
</ul>

<hr>

<h2>Problem Statement</h2>

Urban traffic scenes present significant challenges:

<ul>
<li>High vehicle density</li>
<li>Severe occlusion</li>
<li>Mixed transportation types</li>
<li>Irregular lane discipline</li>
<li>Pedestrian-vehicle interaction</li>
</ul>

This project addresses these challenges using a deep learning-based detection pipeline.

<hr>

<h2>Detected Object Classes</h2>

<ul>
<li>Car</li>
<li>Bus</li>
<li>CNG (Auto-rickshaw)</li>
<li>Motorbike</li>
<li>Bicycle</li>
<li>Pickup</li>
<li>MPV</li>
<li>Rickshaw</li>
<li>Shopping Van</li>
<li>Pedestrian</li>
</ul>

<hr>

<h2>Model Architecture</h2>

<ul>
<li>YOLO-based Improved Detection Model</li>
<li>Anchor-free detection head</li>
<li>Multi-scale feature extraction</li>
<li>Optimized Non-Maximum Suppression</li>
<li>Real-time inference capability</li>
</ul>

<b>Training Configuration:</b>

<ul>
<li>Input Resolution: 640 × 640</li>
<li>Epochs: 50</li>
<li>Batch Size: 8</li>
<li>Early Stopping Enabled</li>
</ul>

<hr>

<h2>Real-World Video Evaluation</h2>

The repository includes three real Dhaka traffic video samples:

<ol>
<li>Incredible Traffic Jam in Dhaka</li>
<li>Traffic Signal in Dhaka City (Part-2)</li>
<li>Traffic Jam in Dhaka City</li>
</ol>

These videos validate:

<ul>
<li>Dense traffic detection</li>
<li>Multi-object simultaneous detection</li>
<li>Pedestrian detection</li>
<li>High occlusion handling</li>
</ul>

<hr>

<h2>Evaluation Metrics</h2>

<ul>
<li>mAP@50</li>
<li>mAP@50-95</li>
<li>Precision</li>
<li>Recall</li>
<li>Confusion Matrix</li>
<li>Per-class mAP</li>
</ul>

<hr>

<h2>Inference Example</h2>

<pre>
results = model.predict(
    source='video_path',
    save=True,
    conf=0.5
)
</pre>

Output:

<ul>
<li>Bounding boxes</li>
<li>Class labels</li>
<li>Confidence scores</li>
<li>Annotated video output</li>
</ul>

<hr>

<h2>Applications</h2>

<ul>
<li>Smart traffic monitoring</li>
<li>Vehicle counting and density estimation</li>
<li>Urban mobility analytics</li>
<li>Intelligent traffic signal systems</li>
<li>Road safety monitoring</li>
</ul>

<hr>

<h2>Repository Structure</h2>

<pre>
├── Traffic_using_Improved_YOLO.ipynb
├── Incredible traffic jam in Dhaka.mp4
├── Traffic Signal In Dhaka City (part-2).mp4
├── Traffic jam in dhaka city.mp4
└── README.md
</pre>

<hr>

<h2>Implementation Notebook</h2>

<a href="https://colab.research.google.com/drive/1VxfdNGWPOPmYGHfwjBrpGH83sB9Ee-jr?usp=sharing">
View Full Colab Implementation
</a>

<hr>

<h2>Author</h2>

<b>Monowar Islam</b><br>
BSc Computer Science and Engineering<br>
Deep Learning | Computer Vision | Intelligent Systems
