# Binary Classification of ADHD and Co-occurring Conditions

This project presents a **Binary Classification Tree** model to analyze the associations between adults diagnosed with **ADHD** and co-occurring conditions, specifically **anxiety** and **substance abuse**, using machine learning techniques in **Python**.

Main [Research Report](https://github.com/AICarope/Binary-Classification-Tree-based-machine-learning-model-Project/blob/main/Project%20Report/Project%203%20Research%20Report.docx)

## Abstract
**ADHD** is a chronic condition affecting around 3% of the adult population. This disorder significantly impacts social and occupational functions. Common symptoms include hyperactivity, impulsivity, and inattention. The **HYPERAKTIV** dataset was used to explore the relationship between ADHD and co-occurring conditions like anxiety and substance abuse.

Two models were developed:
- **Model 1:** Predicts the presence of **substance abuse**.
- **Model 2:** Predicts the presence of **anxiety**.

The models were built using **AdaBoostClassifier** and **RandomForestClassifier**, achieving an accuracy of **81.48%** for **substance abuse** prediction. However, anxiety prediction requires further refinement due to a lower **F1 Score**.

## Dataset
The dataset used in this analysis is the **HYPERAKTIV** dataset, containing health, activity, and heart rate data for:
- 51 adult patients diagnosed with **ADHD**
- 52 clinical controls (total **103 participants**)

## Models and Results

### Model 1: ADHD and Substance Abuse
- **Accuracy:** 81.48%
- **F1 Score:** 73.1%
- **Confusion Matrix:** `[[22, 0], [5, 0]]`

### Model 2: ADHD and Anxiety
- **Accuracy:** 59.25%
- **F1 Score:** 52.13%
- **Confusion Matrix:** `[[13, 0], [11, 3]]`

### Baseline Models
- **Training Time:** 0.003s (substance) and 0.004s (anxiety)
- **Prediction Time:** 0.001s (substance) and 0.001s (anxiety)

## Conclusion
The results show a moderate predictive performance for both models. Further refinement, such as feature engineering, hyperparameter tuning, and exploring ensemble methods, is recommended to improve prediction, especially for anxiety.

## Future Work
Improvements include:
- **Feature Selection:** Add more predictive features related to ADHD, anxiety, and substance abuse.
- **Hyperparameter Tuning:** Apply additional techniques like boosting and bagging to improve model performance.
- **Expanded Data:** Increase the dataset size to include more varied cases and reduce potential overfitting.
