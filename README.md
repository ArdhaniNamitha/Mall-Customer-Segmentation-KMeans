# Mall-Customer-Segmentation-KMeans


This project applies the **K-Means Clustering** algorithm to segment mall customers based on their **Annual Income** and **Spending Score**. The goal is to identify customer groups that share similar purchasing characteristics and help businesses target them more effectively.

---

## Objective

To explore customer data using unsupervised learning and:

* Identify distinct customer profiles
* Group customers with similar spending habits
* Support business decisions like targeted marketing and promotions

---

## Overview

This implementation follows the exact steps required by the task:

1. Load and inspect the dataset
2. Select and scale relevant features
3. Use the Elbow Method to determine the optimal number of clusters
4. Fit the K-Means model
5. Assign cluster labels and visualize results
6. Evaluate the clustering performance using the Silhouette Score

---

## Dataset

* **File**: [dataset(Mall\_Customers).csv](dataset%28Mall_Customers%29.csv)
* **Features used**:

  * `Annual Income (k$)`
  * `Spending Score (1–100)`

These features provide insight into the financial and behavioral characteristics of customers.

---

## Repository Contents

| File Name                                                       | Description                                          |
| --------------------------------------------------------------- | ---------------------------------------------------- |
| [code(Task8).ipynb](code%28Task8%29.ipynb)                      | Jupyter notebook with full clustering implementation |
| [code(task8).py](code%28task8%29.py)                            | Python script version of the notebook                |
| [dataset(Mall\_Customers).csv](dataset%28Mall_Customers%29.csv) | Customer dataset used in this project                |
| [elbow curve.png](elbow%20curve.png)                            | Elbow Method plot for choosing optimal K             |
| [customer segments.png](customer%20segments.png)                | Final cluster visualization showing customer groups  |

---

## Visualizations

### Elbow Method Plot

Used to determine the optimal number of clusters:
[**View Elbow Curve →**](elbow%20curve.png)

### Customer Segmentation Plot

Visual representation of clustered customer segments:
[**View Customer Segments →**](customer%20segments.png)

---

## Evaluation

* **Silhouette Score**: Used to evaluate the tightness and separation of the clusters.
* **Result**: A score of approximately **0.55** indicates that the clusters are reasonably well separated.

---

## How to Run the Project

**Using Google Colab**:

1. Open [code(Task8).ipynb](code%28Task8%29.ipynb) in [Google Colab](https://colab.research.google.com/)
2. Upload [dataset(Mall\_Customers).csv](dataset%28Mall_Customers%29.csv) when prompted
3. Run all cells sequentially to generate results

**Or Locally**:

1. Make sure the required packages are installed:

   ```bash
   pip install pandas matplotlib scikit-learn
   ```
2. Run the script:

   ```bash
   python code(task8).py
   ```

---

## Results

* **Optimal number of clusters**: 5
* Clusters helped identify:

  * High-income, high-spending customers
  * Low-income, low-spending customers
  * High-income but low-spending customers (potential opportunity group)
* These groupings can be used for personalized offers and retention campaigns

---

## Future Improvements

* Add demographic features like Age and Gender
* Use PCA for better visualization in higher dimensions
* Compare K-Means with other clustering methods like DBSCAN or Agglomerative Clustering

