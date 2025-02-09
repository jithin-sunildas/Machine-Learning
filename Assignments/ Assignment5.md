Clustering Algorithms - Iris Dataset

📌 Objective

This project applies clustering techniques to the Iris dataset using K-Means Clustering and Hierarchical Clustering. The goal is to explore how these algorithms group similar data points without labels.

📂 Dataset

Dataset Used: Iris Dataset (from sklearn.datasets)

Features: Sepal length, Sepal width, Petal length, Petal width

Target Variable: Removed (since this is an unsupervised learning problem)

⚙️ Installation

Ensure you have Python and the required libraries installed.

pip install numpy pandas matplotlib seaborn scikit-learn

🚀 Usage

Run the Jupyter Notebook or execute the script to apply the clustering algorithms.

jupyter notebook clustering.ipynb

🏆 Clustering Algorithms Implemented

1️⃣ K-Means Clustering

How it Works:

Assigns data points to k clusters by minimizing the variance within each cluster.

Iteratively updates centroids until convergence.

Why K-Means for Iris Dataset?

The dataset has well-separated clusters, making K-Means effective.

Works well for structured, numerical datasets.

2️⃣ Hierarchical Clustering (Agglomerative)

How it Works:

Initially, each data point is its own cluster.

Iteratively merges the closest clusters based on linkage criteria (Ward’s method).

Forms a hierarchy that can be visualized using a dendrogram.

Why Hierarchical Clustering for Iris Dataset?

Provides a clear hierarchy of clusters.

Useful when the number of clusters is unknown.

📊 Results & Visualization

Elbow Method is used to find the optimal number of clusters for K-Means.

Scatter plots show the clusters identified by both methods.

📌 Notes

The dataset is standardized before clustering to improve performance.

The results may vary slightly due to random initialization in K-Means.
