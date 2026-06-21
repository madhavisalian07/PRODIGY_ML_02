# PRODIGY_ML_02

## Customer Segmentation Using K-Means Clustering
**Internship Domain:** Machine Learning  
**Organization:** Prodigy InfoTech  
**Task Number:** 02  

---

### 1. Project Objective
The primary objective of this task is to implement a K-Means Clustering algorithm to segment customers of a retail store based on their purchase history. By grouping customers with similar behaviors, businesses can optimize targeted marketing strategies and enhance customer satisfaction.

### 2. Dataset & Features Used
The dataset used for this project is `Mall_Customers.csv`. The clustering model relies on the following key metrics to identify distinct consumer behaviors:
* **Annual Income (k$):** The annual earning of the customer.
* **Spending Score (1-100):** A score assigned by the mall based on customer behavior and spending nature.

### 3. Workflow & Methodology
1. **Exploratory Data Analysis (EDA):** Loaded and inspected the structural dimensions of the dataset using Pandas.
2. **Feature Extraction:** Segmented the core feature matrix matrix $X$ using `Annual Income` and `Spending Score` to visualize clear groupings.
3. **Optimizing Clusters (The Elbow Method):** Computed the Within-Cluster Sum of Squares (WCSS) across values of $K$ ranging from 1 to 10 to mathematically determine the optimal inflection point (Elbow), which revealed **$K = 5$**.
4. **Model Architecture:** Implemented the `KMeans` algorithm from `scikit-learn` with `init='k-means++'` to guarantee stable centroid initialization.
5. **Visualization:** Plotted a comprehensive 2D scatter plot representing the 5 distinct consumer archetypes along with their respective centroids.

### 4. Identified Customer Clusters
The model successfully partitioned the shopper base into 5 distinct clusters:
1. **Cluster 1 (Careful):** High income, low spending score.
2. **Cluster 2 (Standard):** Average income, average spending score.
3. **Cluster 3 (Target Group):** High income, high spending score (Highly lucrative for business).
4. **Cluster 4 (Spendthrifts):** Low income, high spending score.
5. **Cluster 5 (Sensible):** Low income, low spending score.

### 5. Core Libraries Applied
* `pandas` & `numpy` - For data manipulation and matrix configurations.
* `scikit-learn` - For implementing the unsupervised K-Means Clustering algorithm.
* `matplotlib` & `seaborn` - For rendering the Elbow curve and cluster scatter plots.

---
**Status:** Completed successfully! 🚀
