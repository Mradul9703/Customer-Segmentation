# Customer Segmentation using Clustering

This project focuses on segmenting customers based on their purchasing behavior using unsupervised machine learning techniques. The goal is to help businesses better understand their customers and develop targeted marketing strategies.

---

## Project Description

Customer segmentation is the process of dividing a customer base into groups of individuals with similar characteristics. In this project, we use clustering algorithms on transaction data to identify distinct groups of customers. The dataset is sourced from an online retail store and includes information such as InvoiceNo, CustomerID, Quantity, UnitPrice, and InvoiceDate.

We calculate RFM (Recency, Frequency, Monetary) features for each customer and apply several clustering algorithms to group them. We also evaluate the performance of clustering using silhouette scores and visualize the clusters.

---

## Dataset

The dataset used is the Online Retail dataset, which contains transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based online retailer.

Features include:
- InvoiceNo: Unique number for each invoice
- StockCode: Product code
- Description: Product name
- Quantity: Number of items purchased
- InvoiceDate: Date and time of the invoice
- UnitPrice: Price per item
- CustomerID: Unique identifier for each customer
- Country: Country name

---

## Technologies Used

- **Programming Language**: Python

- **Environment**: Google Colab

- **Libraries**:
  - `pandas`, `numpy` – for data loading, cleaning, and RFM feature engineering
  - `matplotlib`, `seaborn`, `plotly` – for visualizing distributions and clusters
  - `scikit-learn` – for scaling (`StandardScaler`), clustering (`KMeans`, `AgglomerativeClustering`, `DBSCAN`) and evaluation (`silhouette_score`)
  - `openpyxl` – for reading Excel files in `.xlsx` format

---

## Workflow

1. **Data Loading and Cleaning**
   - Load dataset using pandas
   - Remove missing values and invalid transactions

2. **Feature Engineering**
   - Calculate RFM (Recency, Frequency, Monetary) features
   - Normalize features using StandardScaler

3. **Clustering**
   - Apply multiple clustering algorithms:
     - KMeans
     - Agglomerative Clustering
     - DBSCAN
   - Determine the optimal number of clusters using the elbow method and silhouette scores

4. **Evaluation and Visualization**
   - Use silhouette scores to compare clustering performance
   - Plot 2D clusters using Matplotlib

---

## Results

- KMeans and DBSCAN performed well in distinguishing distinct customer groups.
- Clusters revealed segments such as high-value repeat customers, low-value one-time buyers, etc.
- PCA plots demonstrated good separation between clusters.

---

## Usage

1. Open the notebook `Customer_Segmentation.ipynb` in Jupyter or Colab.
2. Execute the cells in order.
3. Review clustering visualizations and results in the later sections.

---
