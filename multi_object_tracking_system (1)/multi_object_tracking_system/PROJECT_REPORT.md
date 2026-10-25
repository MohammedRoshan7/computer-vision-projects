# Multi-Object Tracking System — Project Report

## Introduction
Multi-object tracking is a computer vision technique that detects objects
and maintains their identities across video frames.

## Objective
To track multiple objects in a video and generate an annotated video and
structured tracking records.

## Methodology
A pretrained YOLO model detects objects. ByteTrack associates detections
across frames. OpenCV handles video input and output, while CSV files store
the tracking records.

## Tools Used
Python, Google Colab, Ultralytics YOLO, ByteTrack, and OpenCV.

## Results
The annotated video is saved in results/tracked_output.mp4.
Tracking records are saved in results/tracking_results.csv.
Processing statistics are saved in results/performance_summary.txt.

## Performance Evaluation
The summary reports processing speed, elapsed time, frames processed, and
unique track IDs observed. These statistics do not measure tracking accuracy.
Formal metrics such as HOTA, IDF1, or MOTA require ground-truth annotations.

## Limitations
Tracking IDs may change when objects overlap or disappear. Performance also
depends on image quality, lighting, and the camera angle.

## Future Improvements
- Evaluate using an annotated tracking dataset.
- Calculate formal tracking metrics.
- Add vehicle counting.
- Test on videos containing crowded scenes.

## Conclusion
The project demonstrates a basic multi-object tracking pipeline using
YOLO and ByteTrack.
