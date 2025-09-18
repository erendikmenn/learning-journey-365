# A Comprehensive Summary of Machine Learning Concepts



> This document provides a foundational overview of core machine learning paradigms, data preparation processes, model evaluation techniques, and fundamental algorithms.



---



## Core Learning Paradigms



### **Supervised Learning**



A method where a model is trained using a dataset containing both known inputs and corresponding outputs. When the trained model is given a new input, it makes a prediction for the output.



-   **Example:** A model can be trained with Audi car price data from 2010-2013 to predict prices for 2014 and beyond. In this simple case, the input is the 'year' and the output is the 'price'. In reality, more features like mileage, model, and vehicle type would be included as inputs.

-   **Common Algorithms:** Regression Analysis, Decision Trees, K-Nearest Neighbors (KNN), Artificial Neural Networks (ANN), and Support Vector Machines (SVM).



### **Unsupervised Learning**



A type of learning where input data is not labeled, meaning the output values are unknown. The primary goal is to discover hidden patterns and structures within the input data.



-   **Example:** Consider the shopping data of thousands of customers without any pre-existing segmentation. Unsupervised learning can analyze this data to identify groups such as "customers who only buy baby products on weekends" or "customers who prefer discounted items at night."

-   **Use Cases:** Frequently used in areas like fraud detection and customer segmentation. The model learns normal behavior patterns and flags deviations.



### **Semi-Supervised Learning (Yarı Gözetimli Öğrenme)**



A method that utilizes a combination of a small amount of labeled data and a large amount of unlabeled data.



-   **Process:** Initially, the model is trained on the small labeled dataset (supervised learning phase). This smarter model then predicts labels for the remaining unlabeled data. Finally, the model is retrained on the now fully labeled, larger dataset to achieve better performance.



### **Reinforcement Learning**



An approach where a model learns to make the best decisions towards a goal through trial and error, guided by a system of rewards and penalties.



-   **Example:** A self-driving car in a simulation environment receives a penalty score (e.g., -1000) for crashing and a reward score (e.g., +100) for reaching its destination. Over time, the model learns that crashing is bad and reaching the goal is good.

-   **Q-Learning:** In this method, an agent records the potential outcome of every action in a table (the Q-table). For instance, a robot might assign -100 points to a step that leads into a fire pit, +100 to a step that reaches treasure, and -1 to every step taken to encourage finding the shortest path. Ultimately, it uses this table to choose the path that yields the highest total score.



---



## Data and Preparation Processes



### **Data Types**



-   **Structured Data:** Clean, organized data in a tabular format, such as customer lists or bank records.

-   **Unstructured Data:** Raw and unorganized data, such as chat logs or videos.



### **Tools for Model Training**



-   **Libraries:** To train a model, you need an environment like `Jupyter Notebook` and several key libraries:

    -   `Pandas`: For data cleaning and manipulation.

    -   `NumPy`: For fast numerical operations.

    -   `Scikit-learn`: For pre-built machine learning models.

    -   `Matplotlib`/`Seaborn`: For data visualization.

-   **Hardware (CPU vs. GPU):** Machine learning models consist of thousands of simple, repetitive calculations. While a CPU is designed for complex, serial tasks, a GPU excels at performing thousands of simple tasks in parallel, making it significantly faster and the preferred choice for ML.



### **Data Cleaning and Preprocessing**



-   **Remove Redundant Data:** Columns that are repetitive or contain the same information (e.g., having both a 'Country' and a 'Country Code' column) should be removed to improve model performance, following the "garbage in, garbage out" principle.

-   **Grouping (Binning/Aggregation):** Features (columns) or observations (rows) are sometimes combined to increase efficiency. For example, "Lion" and "Tiger" rows might be aggregated into a single "Predator" category.

-   **One-Hot Encoding:** Since models cannot work with text, categorical data like "Vulnerable" or "Endangered" must be converted into numerical format using 1s and 0s.

-   **Normalization and Standardization:** Numerical features with different scales, like age (20-65) and salary (20,000-250,000), can cause the model to incorrectly assign more importance to larger numbers. To prevent this, techniques like **Normalization** (scaling data to a 0-1 range) or **Standardization** (scaling data to have a mean of 0 and a standard deviation of 1) are used.

-   **Impute Missing Values:** Missing values in a dataset can be filled using the **Mode** (most frequent value) for categorical data or the **Median** (middle value when sorted) for numerical data.



---



## Model Training and Evaluation



-   **Data Splitting and Shuffling:** To accurately measure performance, the dataset is split into a training set (70-80%) and a test set (20-30%). The data must be shuffled before training to prevent any bias from ordering (e.g., alphabetical order).

-   **Performance Metric (MAE):** One common metric is the **Mean Absolute Error (MAE)**, which measures the average magnitude of the errors in a set of predictions, without considering their direction. It shows how much the model's predictions deviate from the actual values on average.

-   **K-Fold Cross-Validation:** Relying on a single train-test split can be misleading. Instead, the dataset is divided into 'k' equal folds. The model is trained 'k' times, with each fold serving as the test set once. The average of the 'k' results provides a much more reliable estimate of the model's true performance.



---



## Foundational Algorithms in Detail



### **Linear Regression**



-   **Objective:** To model the linear relationship between variables by fitting a trend line (hyperplane) that is closest to the data points. The goal is to minimize the total error (residuals) between the data points and this line.

-   **Types:**

    -   **Simple Linear Regression:** Uses a single input variable.

    -   **Multiple Linear Regression:** Uses more than one input variable.

-   **Considerations:** In multiple regression, using highly correlated independent variables (e.g., fuel consumed and fuel remaining) together causes the **Multicollinearity** problem. This is undesirable, and one of these variables should be removed. This correlation can be detected using tools like heatmaps.



### **Logistic Regression**



-   **Objective:** Unlike linear regression, it performs classification by predicting the probability of an event occurring. For example, it answers "Will this customer repay the loan?" with a "Yes" or "No."

-   **Mechanism:** It uses the **Sigmoid function** to transform the output into a probability value between 0 and 1. Based on a set threshold (e.g., 0.5), this probability is then classified as "Yes" (1) or "No" (0).