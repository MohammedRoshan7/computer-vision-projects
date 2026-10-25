# Multi-Object Tracking System

## 1. Problem Statement
Tracking multiple moving objects in a video is useful for traffic monitoring,
surveillance, and understanding object movement. Detecting objects in individual
frames alone does not maintain their identities across the video.

## 2. Objectives
- Detect multiple objects in video frames.
- Assign tracking IDs to detected objects.
- Track objects across consecutive frames.
- Generate an annotated output video.
- Record basic tracking information for evaluation.

## 3. Dataset
Use a short road or traffic video that you are permitted to use.

Optional benchmark dataset:
KITTI Tracking Dataset
https://www.cvlibs.net/datasets/kitti/eval_tracking.php

## 4. Methodology
1. Load a video.
2. Read its frames.
3. Detect objects using a pretrained YOLO model.
4. Associate detections between frames using ByteTrack.
5. Display bounding boxes and tracking IDs.
6. Save the output video.
7. Evaluate the results using suitable metrics when ground-truth annotations are available.

## 5. Tools and Libraries
- Python
- Google Colab
- Ultralytics YOLO
- ByteTrack
- OpenCV
- NumPy

## 6. Results
Include the annotated tracking video, sample screenshots, and tracking results.

## 7. Performance Evaluation
Report the number of frames processed and processing speed.
For formal tracking evaluation, use ground-truth annotations and suitable metrics,
such as HOTA, IDF1, or MOTA.

## 8. Conclusion
This project demonstrates multi-object detection and tracking using YOLO and ByteTrack.
