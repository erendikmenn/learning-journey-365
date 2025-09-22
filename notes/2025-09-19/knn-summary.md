# Day 2: K-Nearest Neighbors (KNN)

> A summary of the K-Nearest Neighbors algorithm, a distance-based method for classification.

---

### **Core Concept**

-   **Mechanism:** KNN classifies a new data point by examining the classes of its "k" nearest neighbors in the existing dataset.
-   **Majority Vote:** A majority vote is held among these 'k' neighbors, and the new data point is assigned to the most common class.

### **Key Considerations**

-   **Data Scaling:** It is crucial to scale the data before training a KNN model. Because the algorithm is distance-based, features with large numerical ranges can disproportionately influence the distance calculation and dominate the model's outcome.
-   **Choosing 'k':**
    -   An odd number for 'k' is generally preferred to prevent ties during the voting process.
    -   The default value for 'k' in many libraries is 5.

### **Weaknesses**

-   **Performance:** The algorithm's performance can decrease on datasets with a high number of features or a very large number of data points.
-   **Computationally Expensive:** It can be slow because it requires calculating the distance to every training point for each new prediction.
