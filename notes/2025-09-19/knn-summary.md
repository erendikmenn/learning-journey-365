# Day 2: K-Nearest Neighbors (KNN)

> A summary of the K-Nearest Neighbors algorithm, a distance-based method for classification.

---

### **Core Concept**

-   [cite_start]**Mechanism:** KNN classifies a new data point by examining the classes of its "k" nearest neighbors in the existing dataset[cite: 1874].
-   [cite_start]**Majority Vote:** A majority vote is held among these 'k' neighbors, and the new data point is assigned to the most common class[cite: 1875].

### **Key Considerations**

-   [cite_start]**Data Scaling:** It is crucial to scale the data before training a KNN model[cite: 1876]. [cite_start]Because the algorithm is distance-based, features with large numerical ranges can disproportionately influence the distance calculation and dominate the model's outcome[cite: 1876, 1877].
-   **Choosing 'k':**
    -   [cite_start]An odd number for 'k' is generally preferred to prevent ties during the voting process[cite: 1879].
    -   [cite_start]The default value for 'k' in many libraries is 5[cite: 1881].

### **Weaknesses**

-   [cite_start]**Performance:** The algorithm's performance can decrease on datasets with a high number of features or a very large number of data points[cite: 1878].
-   [cite_start]**Computationally Expensive:** It can be slow because it requires calculating the distance to every training point for each new prediction[cite: 1881].