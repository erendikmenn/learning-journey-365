# Day 2: Advanced Model Metrics (StatQuest Summary)

> A summary of advanced classification metrics derived from the confusion matrix: Sensitivity and Specificity. [cite_start]These are used to gain a deeper understanding of model performance, often within a cross-validation framework[cite: 1882, 1884, 1889].

---

### **Definitions and Formulas**

-   [cite_start]**Sensitivity (True Positive Rate):** Measures how well the model correctly identifies actual positive cases[cite: 1892].
    -   [cite_start]**Formula:** `Sensitivity = True Positives / (True Positives + False Negatives)` [cite: 1893]
-   [cite_start]**Specificity (True Negative Rate):** Measures how well the model correctly identifies actual negative cases[cite: 1892].
    -   [cite_start]**Formula:** `Specificity = True Negatives / (True Negatives + False Positives)` [cite: 1890, 1891]

### **Case Study: Choosing the Right Model**

[cite_start]Imagine we need to compare two models, a **Logistic Regression** and a **Decision Tree**, for a critical task like airport security[cite: 1896, 1897, 1898].

-   [cite_start]**The Goal:** The priority is to correctly identify dangerous items (True Positives) and avoid missing any (False Negatives)[cite: 1909]. [cite_start]Therefore, the best model is the one with the higher **Sensitivity**[cite: 1905, 1906, 1907].
-   **The Data:**
    -   [cite_start]**Logistic Regression:** TP=100, FP=5, FN=5, TN=90 [cite: 1899]
    -   [cite_start]**Decision Tree:** TP=90, FP=5, FN=5, TN=100 [cite: 1903]
-   **The Results:**
    -   [cite_start]**Logistic Regression:** Sensitivity = 0.95, Specificity = 0.94 [cite: 1904]
    -   [cite_start]**Decision Tree:** Sensitivity = 0.94, Specificity = 0.955 [cite: 1904]

#### **Conclusion**

[cite_start]For a task where identifying positive cases is critical, the **Logistic Regression model is the better choice** because it has a higher Sensitivity score (0.95)[cite: 1909, 1910, 1912].
