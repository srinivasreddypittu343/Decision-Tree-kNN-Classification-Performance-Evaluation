# Decision-Tree---kNN-Classification---Performance-Evaluation

## 📝 Overview  
This repository contains **three Jupyter notebooks** demonstrating supervised learning techniques using **scikit-learn** on the Iris dataset.  
The focus is on **Decision Trees**, **k-Nearest Neighbors (kNN)**, and **Performance Evaluation** using metrics like **Accuracy, Precision, Recall, F1-score, and ROC/AUC**.  

Each notebook is structured with **step-by-step explanations, visualizations, and analysis** of concepts such as **underfitting, overfitting, model complexity, and decision boundaries**.

---

**Name:** Srinivas Reddy Pittu  
**ID:** 700777009  

---

# 📘 Notebooks Overview  

## 1. `DecisionTree_sklearn.ipynb`  
**Goal:** Explore Decision Trees for classification on the Iris dataset.  

### Steps  
- Load the Iris dataset and split into training and testing sets.  
- Train `DecisionTreeClassifier` models with `max_depth = 1, 2, 3`.  
- Evaluate training and test accuracy for each depth.  
- Discuss **underfitting vs. overfitting** based on accuracy gaps.  
- Visualize trained decision trees and their decision regions.  

### Key Insights  
- **Depth=1:** Underfits → low accuracy on both training and test data.  
- **Depth=2–3:** Balanced performance with good generalization.  
- **Higher depths:** Risk of overfitting when training accuracy far exceeds test accuracy.  

---

## 2. `kNN_Classification_sklearn.ipynb`  
**Goal:** Analyze the impact of **k** in k-Nearest Neighbors classification.  

### Steps  
- Select two Iris features (sepal length, sepal width) for visualization.  
- Train `KNeighborsClassifier` models with `k = 1, 3, 5, 10`.  
- Plot decision boundaries for each **k**.  
- Compare how boundaries evolve as **k** increases.  

### Key Insights  
- **k=1:** Very flexible, jagged decision boundaries → low bias, high variance (overfitting risk).  
- **k=3,5:** Smoother boundaries, better balance between bias and variance.  
- **k=10:** Very smooth boundaries → can underfit by oversimplifying decision regions.  

---

## 3. `Performance_Evaluation.ipynb`  
**Goal:** Evaluate classifier performance using multiple metrics.  

### Steps  
- Train a kNN model with `k=5` on the Iris dataset.  
- Compute and visualize the confusion matrix.  
- Generate a classification report with accuracy, precision, recall, and F1-score.  
- Plot ROC curves (one-vs-rest for multiclass) and calculate AUC.  

### Key Insights  
- **Confusion Matrix:** Shows which classes are often misclassified.  
- **Precision/Recall/F1:** Provide more reliable insights than accuracy, especially for imbalanced datasets.  
- **ROC & AUC:** Useful for visualizing trade-offs between sensitivity and specificity. Multiclass handled via one-vs-rest.  

---
