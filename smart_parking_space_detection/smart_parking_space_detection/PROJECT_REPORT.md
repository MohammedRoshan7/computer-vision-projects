# Smart Parking Space Detection — Project Report

## 1. Introduction
Smart parking systems use computer vision to estimate parking-space
availability and help drivers identify vacant spaces.

## 2. Objective
To identify predefined parking spaces in an image and estimate whether
each space is occupied or available.

## 3. Methodology
The input image is loaded using OpenCV. Parking-space regions are defined
using rectangular coordinates. Canny edge detection is applied to each
region, and edge density is used as a basic occupancy indicator.
The result is displayed using colored rectangles and saved as a CSV file.

## 4. Tools Used
Python, Google Colab, OpenCV, NumPy, and pandas.

## 5. Results
The annotated parking-lot image is saved in results/parking_result.jpg.
The estimated status of each parking space is saved in results/parking_status.csv.

## 6. Performance Evaluation
The number of predicted occupied and available spaces is reported.
For accuracy evaluation, compare predictions against manually labeled
parking-space statuses and calculate accuracy, precision, recall, and F1-score.

## 7. Limitations
The edge-density method is sensitive to shadows, lighting, road markings,
camera angle, and the selected threshold. Parking-space coordinates must
be defined for each image. It may not work reliably on unseen parking lots.

## 8. Future Improvements
- Train a model using labeled parking-space images.
- Test on multiple parking lots and lighting conditions.
- Automate parking-space identification.
- Process video frames to monitor occupancy over time.
- Evaluate performance using labeled ground truth.

## 9. Conclusion
This project demonstrates a basic computer vision approach to estimating
parking-space occupancy using OpenCV.
