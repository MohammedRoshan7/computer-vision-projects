# Multi-Object Tracking System Using YOLO and ByteTrack

## 1. Problem Statement
Detecting objects in individual video frames does not preserve their identities
across time. Multi-object tracking combines object detection with tracking
algorithms to follow objects across consecutive frames.

## 2. Objectives
- Detect multiple objects in video frames.
- Assign tracking IDs to detected objects.
- Track objects across consecutive frames.
- Save an annotated output video.
- Record tracking results in CSV format.

## 3. Dataset
Use a short road or traffic video that you have permission to use.

Optional benchmark:
KITTI Tracking Dataset
https://www.cvlibs.net/datasets/kitti/eval_tracking.php

## 4. Methodology
1. Load a video.
2. Read its frames using OpenCV.
3. Detect objects using a pretrained YOLO model.
4. Associate detections using ByteTrack.
5. Display bounding boxes and tracking IDs.
6. Save the output video and tracking records.
7. Evaluate against ground-truth annotations when available.

## 5. Tools and Libraries
- Python
- Google Colab
- Ultralytics YOLO
- ByteTrack
- OpenCV
- NumPy
- Pandas

## 6. Results
See the results folder for the tracking video, CSV records, and evaluation summary.

## 7. Performance Evaluation
The program records processed frames, elapsed time, processing speed, and the
number of unique track IDs observed. These are descriptive statistics, not
formal tracking accuracy metrics.

Formal metrics such as HOTA, IDF1, and MOTA require ground-truth annotations.

## 8. Limitations
Tracking IDs can change when objects overlap, disappear, or are missed.
Performance depends on video quality, lighting, and camera angle.

## 9. Conclusion
This project demonstrates multi-object tracking using YOLO and ByteTrack.
