Spotify Playlist Clustering — Moosic Prototype

Overview

In this project, we explored unsupervised machine learning techniques to create meaningful playlists from 5,000 Spotify songs.
The goal was to cluster songs based on their audio features and discover hidden patterns without any predefined labels.

What We Learned

1. Data Scaling
Before clustering, we scaled the features to bring them onto a similar scale.
We used three types of scaling methods:

Standard Scaler (Standardization),
MinMax Scaler (Normalization),
Robust Scaler

2. Data Transformation
To handle non-linear distributions and improve clustering results, we also applied two transformations:

Quantile Transformation,
Power Transformation

3. Dimensionality Reduction: PCA
We applied Principal Component Analysis (PCA) to reduce dimensionality while preserving the most important information.
This allowed us to work with fewer, more meaningful components, making clustering more effective and faster.

4. Clustering Techniques
Once we had the transformed and reduced data, we applied clustering techniques:

K-Means Clustering — to form natural song groups based on features.
Silhouette Analysis — to evaluate how well our clusters were separated and to find the ideal number of clusters.
Key Steps

Data Preprocessing: Scaling, transforming, and cleaning the dataset.
Feature Selection: Dropping irrelevant or redundant features (e.g., loudness, time_signature).
Dimensionality Reduction: Applying PCA to find important components.
Clustering: Grouping songs into distinct playlists using K-Means.
Validation: Using Silhouette Score to evaluate clustering quality.
Highlights

Successfully divided 5,000 songs into 34 distinct clusters.
Each cluster represents a unique musical "playlist" based on shared audio features.
Visualized clusters using colorful PCA scatterplots.
Created a strong foundation for auto-generating curated playlists.
Next Steps

Explore more clustering algorithms (DBSCAN, Hierarchical Clustering).
Incorporate user behavior data (likes, skips, replays).
Improve cluster naming using NLP on lyrics or song metadata.
Deploy an interactive dashboard for playlist exploration.

Technologies Used

Python (Pandas, Numpy)
Scikit-learn
Seaborn, Matplotlib
Plotly
Google Colab
