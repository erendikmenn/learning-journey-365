# Bias and Variance

> A summary of the concepts of bias and variance, which explain a model's performance.

---

### **Core Concepts**

* [cite_start]**Bias:** A model with high **bias** is too simple and doesn't fit the training data well[cite: 52]. [cite_start]This often happens with linear regression models[cite: 46, 52]. [cite_start]A model with high bias might perform well on test data because its results are consistent[cite: 6].
* [cite_start]**Variance:** A model with high **variance** fits the training data perfectly but performs very poorly on test data[cite: 6]. [cite_start]This suggests the model is overly complex and has essentially memorized the training data[cite: 53].

### **Addressing Bias and Variance**

There are several methods to deal with the trade-off between bias and variance:

* [cite_start]**Regularization:** This method works by restricting the parameters of overly complex models to reduce their variance[cite: 7].
* [cite_start]**Boosting:** This technique combines multiple weak models to create a more effective, single model[cite: 8].
* [cite_start]**Bagging:** This method combines the predictions from multiple models to reduce variance[cite: 9].