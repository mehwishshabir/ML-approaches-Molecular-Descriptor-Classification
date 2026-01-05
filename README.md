# Machine Learning Approaches Used in Classifiying the Molecular Descriptors – WEKA-Based Study

## Project Overview
This project explores the application of various Machine Learning (ML) algorithms in the field of Drug Design using the **WEKA Explorer**. The goal is to classify chemical compounds based on their molecular descriptors (CDD_2D dataset) and compare the efficiency of different classification models.

## Methodology
The dataset was pre-processed by removing attributes with a high percentage of zero values to reduce noise and prevent overfitting. The classification was performed using an 85% training and 15% testing split.
## Algorithms Used
- k-Nearest Neighbors (IBk)
- Decision Tree (J48)
- Support Vector Machine (SMO)
- Artificial Neural Network (Multilayer Perceptron)

## Tools
- WEKA Explorer (GUI-based ML)
- descriptor dataset

## Evaluation Strategy
- Percentage split (85/15 and 66/34)
- Accuracy, TP rate, FP rate


## Key Findings
- KNN (k=3, Manhattan distance) achieved the best performance
- Decision trees showed overfitting with low minNumObj
- SVM kernel choice significantly impacted accuracy
- ANN was slowest and sensitive to hyperparameters
