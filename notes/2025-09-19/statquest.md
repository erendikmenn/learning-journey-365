# Day 2: Advanced Model Metrics (StatQuest Summary)

> A summary of advanced classification metrics derived from the confusion matrix: Sensitivity and Specificity. These are used to gain a deeper understanding of model performance, often within a cross-validation framework[cite: 1882, 1884, 1889].

---

### **Definitions and Formulas**

-   **Sensitivity (True Positive Rate):** Measures how well the model correctly identifies actual positive cases.
    -   **Formula:** `Sensitivity = True Positives / (True Positives + False Negatives)` 
-   **Specificity (True Negative Rate):** Measures how well the model correctly identifies actual negative cases.
    -   **Formula:** `Specificity = True Negatives / (True Negatives + False Positives)` 

### **Case Study: Choosing the Right Model**

Imagine we need to compare two models, a **Logistic Regression** and a **Decision Tree**, for a critical task like airport security.

-   **The Goal:** The priority is to correctly identify dangerous items (True Positives) and avoid missing any (False Negatives). Therefore, the best model is the one with the higher **Sensitivity**.
-   **The Data:**
    -   **Logistic Regression:** TP=100, FP=5, FN=5, TN=90 
    -   **Decision Tree:** TP=90, FP=5, FN=5, TN=100 
-   **The Results:**
    -   **Logistic Regression:** Sensitivity = 0.95, Specificity = 0.94 
    -   **Decision Tree:** Sensitivity = 0.94, Specificity = 0.955 

#### **Conclusion**

For a task where identifying positive cases is critical, the **Logistic Regression model is the better choice** because it has a higher Sensitivity score (0.95).
