

# DonorsChoose Clustering Analysis

This project applies various clustering algorithms to group DonorsChoose project proposals based on their text and metadata, aiming to identify patterns in project approvals.

## Dataset
- **DonorsChoose.org Project Proposals**.
- **Features**: Project titles, essays, grade categories, subject categories, resource summaries, and teacher information.
- **Target**: Project approval (binary classification).

## Key Steps
1. **Data Preprocessing**:
   - Cleaned and vectorized text features (project essays, titles) using Bag of Words (BOW) and TF-IDF.
   - Applied one-hot encoding to categorical features like project categories and teacher prefixes.

2. **Clustering Methods**:
   - **K-Means Clustering**: Used the elbow method to identify the optimal number of clusters.
   - **Agglomerative Clustering**: Applied hierarchical clustering on a subset of the data.
   - **DBSCAN**: Used the elbow method to find the optimal distance for clustering.

3. **Dimensionality Reduction**:
   - Applied **Truncated SVD** to reduce the dimensionality of the dataset for visualization.
   - Visualized clusters in 2D space using scatter plots.

4. **Word Clouds**:
   - Generated word clouds for each cluster to summarize the most frequent terms.

## Results
- **Optimal Clusters**: Found 4 optimal clusters using K-Means, and 2 clusters using Agglomerative Clustering.
- **Cluster Analysis**: Word clouds and text analysis helped identify distinct themes within each cluster, such as project types and resource needs.

## Conclusion
Clustering provided valuable insights into different groups of projects on DonorsChoose, helping to identify common characteristics and areas where projects might need further review or approval assistance.
