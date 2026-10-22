# Motor Bearing Fault Diagnosis Using Deep Learning

## Overview
A deep learning project that uses a 1D Convolutional Neural Network (CNN) to classify motor bearing conditions from vibration signals. The project explores the use of machine learning for predictive maintenance.

## Problem Statement
Motor bearing faults can lead to equipment failure and unplanned downtime. This project investigates whether vibration signal patterns can be used to distinguish normal bearings from common bearing faults.

## Tech Stack
- Python
- TensorFlow / Keras
- NumPy and SciPy
- Matplotlib
- Scikit-learn
- Google Colab

## Dataset
Vibration recordings from the Case Western Reserve University (CWRU) Bearing Data Center.

The model classifies four categories:
- Normal
- Inner-race fault
- Ball fault
- Outer-race fault

Dataset: https://engineering.case.edu/bearingdatacenter/download-data-file

## Approach
1. Loaded vibration signals from MATLAB data files.
2. Divided signals into 1,024-sample windows.
3. Standardized the signal windows.
4. Split original recordings into training, validation, and test sets.
5. Built and trained a 1D CNN using TensorFlow/Keras.
6. Evaluated predictions using classification metrics and a confusion matrix.

## Initial Results
- Test accuracy: **100% on the current test split**
- Evaluation size: 505 signal windows
- Metrics: Precision, recall, F1-score, and confusion matrix

**Note:** The initial evaluation uses a limited number of independent recordings, with one held-out recording per class. Further testing across more recordings and operating conditions is required to assess generalization.

## Future Improvements
- Validate using additional independent recordings.
- Test performance across different operating conditions.
- Compare CNN results with traditional machine learning models.
- Develop an interactive fault-prediction demo.

## Disclaimer
This is an academic portfolio project, not a validated industrial diagnostic system.
