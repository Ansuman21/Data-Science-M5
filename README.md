# **Evaluating and Optimizing Model Performance for Business Decision-Making**

## **Business Case**
The objective of this project was to assess the performance of a binary classification model using various evaluation metrics. In a business scenario, this could apply to industries such as finance, healthcare, or e-commerce, where predicting outcomes accurately is crucial. The classification model is intended to distinguish between two classes (e.g., "Good" vs. "Bad" loan applicants, "Disease Present" vs. "No Disease," etc.). 

The business challenge was to ensure that the model performed well enough to make accurate predictions, minimize false positives and false negatives, and make data-driven decisions. The performance metrics used in this project can directly influence decision-making processes, such as whether or not to approve loan applications or detect disease in patients.

## **Project Overview**
This project evaluates a classification model's performance using several key metrics, including accuracy, precision, recall, F1 score, specificity, and AUC-ROC. The project includes both custom Python functions for evaluation and comparison with scikit-learn's pre-built functions.

## **Key Steps Taken**

### **1. Data Exploration and Preparation**
- The dataset consisted of binary classification labels (0 or 1), and the first step was to explore the data and identify the target variable and features.
- The key metric used was the **scored.probability** column for model predictions and **class** column as the actual outcomes.

### **2. Model Performance Metrics**
Custom Python functions were developed to calculate:
- **Accuracy**: The proportion of correct predictions to the total predictions.
- **Precision**: The proportion of positive predictions that are actually positive.
- **Sensitivity (Recall)**: The proportion of actual positives that are correctly identified.
- **Specificity**: The proportion of actual negatives that are correctly identified.
- **F1 Score**: The harmonic mean of precision and recall, balancing the two metrics.
  
These custom functions were compared with scikit-learn's built-in functions to ensure the accuracy of the calculations.

### **3. ROC Curve and AUC**
- The **ROC Curve** was plotted to assess the model’s discriminative power by visualizing the trade-off between the True Positive Rate (Sensitivity) and the False Positive Rate.
- **AUC (Area Under the Curve)** was calculated to quantify the overall ability of the model to discriminate between classes. A value close to 1 indicates good model performance, while a value close to 0 suggests poor performance.

### **4. Model Evaluation**
- Evaluated the model using the calculated metrics: accuracy, precision, recall, specificity, F1 score, and AUC.
- Plotted the ROC curve and calculated AUC for both custom functions and scikit-learn's functions.
- Compared the custom implementation of ROC curve and AUC with scikit-learn's results to validate the custom calculations.

### **5. Performance Insights**
- **Precision**: The model showed a precision of 84.38%, indicating a relatively good ability to predict positives accurately.
- **Recall (Sensitivity)**: At 47.37%, the recall was lower, meaning the model missed some of the actual positives.
- **F1 Score**: The F1 score was calculated as 60.67%, highlighting the balance between precision and recall.
- **AUC**: The AUC score of 0.85 suggested that the model had a reasonable ability to discriminate between classes.
  
### **6. Comparison with Scikit-learn**
- The scikit-learn library’s functions were used for evaluation, providing results consistent with the custom calculations.
- The AUC value from scikit-learn was found to be 0.85, confirming the model’s reasonable ability to discriminate.
  
### **7. Model Limitations and Next Steps**
- The model, while having a good precision, demonstrated weaknesses in recall and a relatively low F1 score.
- Further steps include improving the feature set, model tuning, and potentially exploring different algorithms.
  
## **Key Findings and Recommendations**
- The model demonstrated better-than-random ability to discriminate between classes, with an AUC of 0.85.
- There was a notable imbalance in precision and recall, with precision being higher than recall. This can be adjusted based on business priorities (e.g., lowering false negatives or false positives).
- Given the low recall, improving the model’s sensitivity (e.g., by adjusting the decision threshold) should be a priority to reduce missed positives.
- Data preprocessing, feature engineering, and additional training are recommended to improve model performance.
- A deeper analysis of the model’s behavior across different thresholds may provide more actionable insights for decision-making.

## **Project Insights**
- The evaluation process helped identify the strengths and weaknesses of the classification model.
- The model showed reasonable discriminative ability, but its recall performance can be improved for better real-world application.

## **Technologies and Tools Used**
- **Python**: For custom calculations and plotting.
- **scikit-learn**: For built-in performance metrics and comparison.
- **Matplotlib**: For plotting the ROC curve.
- **NumPy**: For numerical calculations.
  
## **Author**
**Ansuman Patnaik**  
  MS in Data Science & Analytics, Yeshiva University  
  ansu1p89k@gmail.com
