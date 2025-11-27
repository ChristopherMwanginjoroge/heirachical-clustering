This project performs Agglomerative Hierarchical Clustering to segment customers based on their annual income and spending score.
Hierarchical clustering provides intuitive cluster grouping and a dendrogram that visually shows how clusters form.

The project is ideal for:

Market segmentation

Customer behavior analysis

Unsupervised machine learning practice

🎯 Objectives

Load and preprocess customer data

Use the Ward linkage method to build a hierarchical structure

Visualize the dendrogram to determine the optimal number of clusters

Apply Agglomerative Clustering

Visualize the resulting clusters

Analyze each customer segment

📂 Dataset

Mall Customers Dataset
Download here:
https://www.kaggle.com/datasets/shwetabh123/mall-customers

Features used for clustering:

Annual Income (k$)

Spending Score (1–100)

🧠 Methods & Algorithms
✔️ Agglomerative Hierarchical Clustering

A bottom-up clustering approach where:

Each point starts as its own cluster

Clusters merge step by step

The process continues until the desired number of clusters is formed

We use:

Linkage method: Ward

Distance metric: Euclidean

Number of clusters: Determined using dendrogram (5 clusters)

✔️ Dendrogram

A tree-like diagram showing how clusters merge at each level.
It helps visually determine the number of clusters by identifying the largest vertical gap.

✔️ Scaling

We use StandardScaler to ensure all features contribute equally.

🛠️ Technologies Used

Python

Pandas

NumPy

Scikit-Learn

SciPy (linkage and dendrogram)

Matplotlib

📊 Project Workflow
1. Load the Data

Read the CSV and inspect the dataset.

2. Feature Selection

We select two features to allow clear visualization of clusters.

3. Data Scaling

Agglomerative clustering requires scaled data for proper distance measurement.

4. Dendrogram Creation

We generate a dendrogram using SciPy’s linkage function to determine the number of clusters.

5. Agglomerative Clustering

We fit an AgglomerativeClustering model using the number of clusters chosen from the dendrogram.

6. Cluster Visualization

Clusters are plotted in 2D to show:

Spending patterns

Income distribution

Cluster boundaries

7. Cluster Interpretation

The model typically identifies groups such as:

High-income, high-spending

Low-income, low-spending

High-income, low-spending

Medium segments

These insights are useful for marketing and strategy.
