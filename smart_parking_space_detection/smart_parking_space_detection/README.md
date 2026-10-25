# Smart Parking Space Detection Using Computer Vision

## 1. Problem Statement
Finding available parking spaces can be difficult in busy parking areas.
This project analyzes parking-lot images or video frames to estimate which
predefined parking spaces are occupied and which are available.

## 2. Objectives
- Identify individual parking spaces.
- Classify spaces as occupied or available.
- Display the parking status visually.
- Save annotated output images and parking statistics.

## 3. Dataset
Use a parking-lot image or video that you have permission to use.

Optional dataset:
PKLot Parking Lot Database
https://web.inf.ufpr.br/vri/databases/parking-lot-database/

## 4. Methodology
1. Load a parking-lot image.
2. Define the regions corresponding to individual parking spaces.
3. Extract each parking-space region.
4. Analyze image features to estimate occupancy.
5. Mark each space as occupied or available.
6. Display and save the annotated result.
7. Evaluate against labeled data when available.

## 5. Tools and Libraries
- Python
- Google Colab
- OpenCV
- NumPy
- Matplotlib

## 6. Results
See the results folder for annotated images and parking statistics.

## 7. Performance Evaluation
Record the number of occupied and available spaces.
For accuracy evaluation, compare predictions with manually labeled ground truth.

## 8. Limitations
The simple image-feature method depends on camera angle, lighting, shadows,
and the predefined parking-space regions. It may not generalize to arbitrary
parking lots without recalibration.

## 9. Conclusion
This project demonstrates a basic computer vision approach to parking-space
occupancy estimation.
