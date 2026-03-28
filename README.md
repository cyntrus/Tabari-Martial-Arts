From Pose to Prediction: Classifying Martial Arts Techniques Using
Temporal Deep Learning and Biomechanical Joint Features

Author: Areej Alsini
Email: aosini@uqu.edu.sa

Tabari is a pose-based deep learning framework for the automatic classification of martial arts techniques from video sequences. The framework extracts skeletal pose data using MediaPipe and classifies techniques using three temporal deep learning architectures: Bidirectional Long Short-Term Memory (Bi-LSTM), Temporal Convolutional Network (TCN), and Transformer Encoder.

The dataset provided in this repository contains pose annotations for five martial arts techniques spanning Karate and Taekwondo, and is intended to support reproducibility of the results reported in the associated paper.

Techniques
The dataset covers the following five techniques:
TechniqueMartial ArtMae GeriKarateZukiKarateYop ChagiTaekwondoDwi ChagiTaekwondoDolgae ChagiTaekwondo

Dataset
Description
The dataset consists of pose annotation files in JSON format, extracted from video sequences using MediaPipe Pose. Each JSON file corresponds to a single video clip and contains frame-by-frame skeletal data represented as a 107-dimensional dual feature vector combining:

MediaPipe landmark coordinates (x, y, z, visibility) for 33 body keypoints
Biomechanically meaningful joint angles computed from the skeletal landmarks
