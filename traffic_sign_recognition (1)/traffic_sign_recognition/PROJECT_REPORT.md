# Traffic Sign Recognition — Project Report

## Introduction
Traffic sign recognition is a computer vision task that classifies road
sign images into categories such as speed limits, warnings, and restrictions.

## Objective
To develop and evaluate a CNN model for traffic sign image classification.

## Methodology
Images are resized and normalized before being used to train a CNN.
The trained model predicts a traffic sign category for each input image.

## Implementation
The project uses Python, TensorFlow/Keras, OpenCV, and Google Colab.

## Evaluation
The validation classification report contains precision, recall, F1-score,
and accuracy-related information. Validation results are not a substitute
for evaluation on a separate official test set.

## Limitations
Performance may be affected by image quality, lighting, sign orientation,
and differences between training and real-world images. The model classifies
provided sign images; it does not detect signs in full road scenes.

## Future Improvements
- Evaluate using the official test set.
- Add a confusion matrix.
- Test on images captured from real roads.
- Add a separate object detector to locate signs in full scenes.

## Conclusion
This project demonstrates CNN-based traffic sign image classification.
