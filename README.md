# Machine Learning Approaches for Molecular Descriptors Classification

## Project Overview
This repository presents a comparative study of **Machine Learning (ML)** algorithms applied to **Drug Design**. Using the **WEKA Explorer**, I evaluated how different computational models classify chemical compounds based on their molecular descriptors (CDD_2D dataset). 

The core focus was on balancing model complexity with predictive accuracy and understanding the impact of descriptor pre-processing on classification performance.

* **Platform:** WEKA Explorer (GUI-based Machine Learning)
* **Dataset:** `CDD_2D.arff` (Molecular Descriptors)
* **Pre-processing:** Attributes with high zero-variance were removed to streamline the models, improve computational efficiency, and mitigate the risk of overfitting.
* **Evaluation Strategy:** * Primary split: **85% Training / 15% Testing**.
    * Metrics: Accuracy, True Positive (TP) Rate, False Positive (FP) Rate, and Confusion Matrices.

---

## Algorithms Evaluated
I implemented and tuned four distinct ML paradigms:

1.  **k-Nearest Neighbors (IBk):** Optimized using $k=3$ and Manhattan Distance.
2.  **Decision Tree (J48):** Evaluated through tree visualization and pruning (Size: 115).
3.  **Support Vector Machine (SMO):** Comparative analysis of Poly, Puk, and RBF kernels.
4.  **Artificial Neural Network (Multilayer Perceptron):** Tuned via GUI for Epochs, Learning Rate, and Momentum.
   
---
## Key Findings
Based on the experimental results, **KNN** emerged as the most effective model for this specific molecular dataset.

### Observations:
* **Distance Metrics:** Switching from Euclidean to Manhattan distance in KNN improved accuracy, suggesting Manhattan distance is better suited for high-dimensional descriptor spaces.
* **Overfitting:** In Decision Trees, reducing `minNumObj` to 1 increased tree size but decreased overall accuracy, confirming the risk of overfitting on training noise.
* **Computational Cost:** The Artificial Neural Network was the most computationally intensive approach while showing higher sensitivity to false positives during parameter tuning.

---
## 📂 Repository Contents
* `Report/`: Contains the full project documentation (PDF).
---
## 🔒 Dataset Information
**Note:** The raw training data (`CDD_2D.arff`) is **not included** in this repository due to academic and privacy restrictions. However, all descriptor selection criteria, pre-processing steps, and specific model hyper-parameters are fully detailed in the project report.
