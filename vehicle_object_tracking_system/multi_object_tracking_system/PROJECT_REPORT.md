# Multi-Object Tracking System — Project Report

## Introduction
Multi-object tracking is a computer vision technique used to detect and
follow multiple objects across consecutive video frames.

## Objective
To detect moving objects, assign tracking IDs, and save the tracking
results in an annotated video.

## Methodology
A pretrained YOLO model detects objects in each frame. ByteTrack associates
detections between frames and maintains track identities when possible.
OpenCV reads the input video and saves the processed output.

## Implementation
The project is implemented in Python using Google Colab, Ultralytics YOLO,
ByteTrack, and OpenCV.

## Results
The annotated video is saved as results/tracked_output.mp4.
The detection and tracking records are saved as results/tracking_results.csv.

## Performance Evaluation
The program reports the number of processed frames and unique track IDs
observed. These are basic descriptive statistics, not formal tracking
accuracy measurements. Formal metrics such as HOTA, IDF1, and MOTA require
ground-truth tracking annotations.

## Limitations
Tracking IDs can change when objects overlap, disappear, or are missed.
Results depend on video quality, camera angle, lighting, and model accuracy.

## Future Improvements
- Evaluate the system on an annotated benchmark dataset.
- Calculate formal tracking metrics.
- Improve performance on crowded scenes.
- Add vehicle counting or traffic-flow analysis.

## Conclusion
The project demonstrates a basic multi-object tracking pipeline that
combines object detection with tracking across video frames.
