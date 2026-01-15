Sampling Techniques Performance Analysis




📌 Project Overview

The objective of this assignment is to evaluate the importance of sampling techniques when dealing with
imbalanced datasets. In real-world scenarios, class imbalance can significantly degrade model performance.
This project demonstrates how to balance a dataset and identifies which sampling strategies work best for 
specific machine learning models.




🛠️ Methodology

1. Data Balancing
The original credit card dataset was highly imbalanced. I used the SMOTE
 (Synthetic Minority Over-sampling Technique) to create a balanced class distribution.

2. Sampling Techniques
Five distinct sampling techniques were applied to the balanced data:
Sampling 1: Simple Random Sampling
Sampling 2: Systematic Sampling
Sampling 3: Stratified Sampling
Sampling 4: Cluster Sampling
Sampling 5: Bootstrap Sampling

3. Machine Learning Models
Five different machine learning models were tested:
M1: Extra Trees Classifier
M2: AdaBoost Classifier
M3: Gaussian Naive Bayes
M4: Linear Discriminant Analysis (LDA)
M5: MLP Classifier (Neural Network)





📊 Accuracy Results
The table below shows the accuracy (%) of each model across the five sampling techniques:

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **M1 (ExtraTrees)** | **100.00** | 96.91 | 97.92 | 96.91 | 98.97 |
| **M2 (AdaBoost)** | 95.88 | **96.91** | 91.67 | 95.88 | **96.91** |
| **M3 (NaiveBayes)** | 84.54 | 82.47 | 79.17 | 85.57 | **95.88** |
| **M4 (LDA)** | 89.69 | 85.57 | 87.50 | 87.63 | **96.91** |
| **M5 (MLP)** | 93.81 | 90.72 | 89.58 | 91.75 | **98.97** |





🏆 Final Conclusion (Task 5)
Based on the experimental results:
-Extra Trees (M1) achieved the highest performance with Simple Random Sampling.
-AdaBoost (M2) showed high stability across Systematic and Bootstrap Sampling.
-Gaussian NB, LDA, and MLP all performed exceptionally well with Bootstrap Sampling (Sampling 5).
Overall, Bootstrap Sampling proved to be the most consistent technique for achieving higher accuracy across 
diverse models in this project.

