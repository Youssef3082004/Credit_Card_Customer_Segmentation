# Credit Card Customer Segmentation & Classification
<div align="center">

[![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/jupyter-%23f37726.svg?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-%2311557c.svg?style=for-the-badge&logo=python&logoColor=white)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/seaborn-%230C7BDC.svg?style=for-the-badge&logo=python&logoColor=white)](https://seaborn.pydata.org/)
</div>

## 📌 Overview
This project focuses on analyzing **Credit Card Dataset for Clustering**.  
The workflow is divided into two main parts:
1. **Unsupervised Learning (K-Means Clustering)**  
   - Used to segment customers based on their credit card usage patterns.
   - Achieved **0.32 Silhouette Score for Clustering** 🎯
2. **Supervised Learning (Random Forest Classification)**  
   - Built a classification model on the clustered dataset to predict cluster labels.  
   - Achieved **98.88% accuracy** 🎯.


## 📂 Dataset
- **Source:** [Credit Card Dataset for Clustering **(Kaggle)**](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata)  
- **Description:** Contains anonymized credit card usage data for Customers.  
* Features: 
   - **``TENURE``** 
   - **`BALANCE_RANGE`**
   - **`PURCHASES_RANGE`**
   - **`ONEOFF_PURCHASES_RANGE`**
   - **`INSTALLMENTS_PURCHASES_RANGE`**
   - **`CASH_ADVANCE_RANGE`**
   - **`CREDIT_LIMIT_RANGE`** 
   - **`PAYMENTS_RANGE`** 
   - **`MINIMUM_PAYMENTS_RANGE`**
   - **`BALANCE_FREQUENCY_RANGE`**
   - **`PURCHASES_FREQUENCY_RANGE`**
   - **`ONEOFF_PURCHASES_FREQUENCY_RANGE`**
   - **`PURCHASES_INSTALLMENTS_FREQUENCY_RANGE`**
   - **`CASH_ADVANCE_FREQUENCY_RANGE`**
   - **`PRC_FULL_PAYMENT_RANGE`**
   - **`PURCHASES_TRX_RANGE`** 
   - **`CASH_ADVANCE_TRX_RANGE`**

## 🛠️ Methodology
### 1. Data Preprocessing
- Handled missing values.  
- Standardized numerical features.  
- Prepared dataset for clustering.

### 2. Clustering with K-Means
- Chose optimal **`K`** using the **`Elbow method`**.  
- Segmented customers into clusters.  
- Visualized clusters for interpretation.

### 3. Classification with Random Forest
- Used **`K-Means`** cluster assignments as **pseudo-labels**.  
- Trained a **`Random Forest Classifier`** to predict cluster membership.  
- Evaluated performance with accuracy and classification report.


## 📊 Results
- **Silhouette Score for Clustering:** `0.32` ✅
- **Random Forest Accuracy:** `98.88%` ✅  
- **Classification Report:**
  - Precision, Recall, and F1-score all ≈ `0.99`.  
- Strong evidence that clusters are well-separated and predictable.

## 📈 Visualizations

<div align="center">

<p>
  <img src="assets/elbow.png" alt="Elbow Method Plot" width="600"/>
</p>
<sub>Determining the optimal number of clusters using the WCSS (Elbow) technique.</sub>

---

<p>
  <img src="assets/cluster.png" alt="Clustering Visualization" width="600"/>
</p>
<sub>Visualization of the dataset after applying K-Means clustering.</sub>
</div>



---
<h3 align="center">Developed as an Independent Machine Learning Project</h3>