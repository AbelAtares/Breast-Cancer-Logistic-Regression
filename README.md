# Breast Cancer Logistic Regression

This project implements a predictive model to distinguish between benign and malignant breast tumors using a **Logistic Regression classifier**. The dataset used comes from the **Wisconsin Breast Cancer Database**. The goal is to explore the features, visualize the data, and evaluate the model’s performance in identifying cancerous tumors.

---

## Import and Study Data

- The dataset is loaded and the **target variable is converted into 0s and 1s** for benign and malignant cases.  
- A preliminary study of the feature variables is performed separately for benign and malignant tumors.  
- This helps identify which features are most correlated with the target.  
- Based on the analysis, **`newflayer`** was selected as the most relevant feature for modeling.

---

## Data Visualization

- A **scatter plot** is created to visualize the distribution of the examples.  
- **Transparency (opacity)** is reduced to better distinguish overlapping points between benign and malignant cases.

---

## Data Split

- The dataset is split into **training and test sets**, with **80% for training** and **20% for testing**.  
- This ensures the model is trained on most of the data but evaluated on unseen samples for a realistic performance estimate.

---

## Model Implementation

- A **Logistic Regression model** is defined using **Scikit-learn**.  
- The model is configured to classify tumors based on the selected features.

---

## Prediction

- The trained model is used to **predict labels for the test set**.  
- These predictions are then compared to the actual labels to evaluate the model’s accuracy.

---

## Model Performance

- The model is evaluated using standard metrics:  
  - **Accuracy**  
  - **Precision**  
  - **Recall**  
  - **ROC AUC**  
- Results show that the model performs well overall.  
- **Recall is around 80%**, which indicates some malignant cases may still be misclassified.  
- Since this is a **health-related problem**, improving Recall is critical to reduce the risk of false negatives.

---

**Conclusion:**  
The Logistic Regression model provides a solid baseline for tumor classification. Feature analysis, visualization, and careful evaluation highlight areas where further improvements could be made, particularly in increasing Recall for high-stakes medical applications.
