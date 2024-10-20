# README.md

## Online News Popularity: Visual Analysis

This project demonstrates various approaches to analyzing and visualizing the "Online News Popularity" dataset using clustering techniques and advanced data visualization tools. The analysis focuses on grouping articles based on their content characteristics and exploring the distribution of article shares across different categories and time periods.

### Requirements

Before running the notebook, make sure to install the following Python libraries:

- `pandas`
- `numpy`
- `scikit-learn`
- `plotly`
- `seaborn`
- `matplotlib`

These can be installed using pip:

```bash
pip install pandas numpy scikit-learn plotly seaborn matplotlib
```

### Dataset

The dataset used in this notebook is the **Online News Popularity** dataset. You can download the dataset from [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/online+news+popularity).

Make sure to place the dataset (CSV file) in the same directory as this notebook, or update the file path accordingly.

### Key Features

1. **Data Preprocessing:**
   - The dataset is preprocessed by selecting relevant numerical and categorical features for analysis.
   - Features are normalized, and irrelevant columns are removed to streamline the analysis.

2. **Clustering Analysis:**
   - **KMeans Clustering**: We perform KMeans clustering on selected features, including `n_tokens_content`, `num_imgs`, and `num_videos`, and also explore other feature combinations.
   - **Silhouette Analysis**: We calculate silhouette scores to measure the quality of clustering for different approaches, identifying the best combination of features and clusters.

3. **Principal Component Analysis (PCA):**
   - PCA is applied to reduce dimensionality and improve clustering performance by capturing the most important features.

4. **Visualization:**
   - We use **Plotly** and **Seaborn** to create dynamic visualizations of the dataset:
     - 3D scatter plots showing clusters of articles based on content characteristics.
     - Violin plots and bar charts to explore the distribution of article shares across different days of the week and content channels.
     - Correlation heatmaps to analyze relationships between content categories and shares.

5. **Visualization of Clusters:**
   - Each clustering approach is visualized using 3D scatter plots to illustrate how articles are grouped based on different content and share characteristics.
   - Pair plots and silhouette coefficient plots are used to evaluate the clustering results.

### Clustering Approaches

1. **Approach 1:**
   - Clustering based on content features such as the number of tokens, images, and videos in each article.

2. **Approach 2:**
   - Clustering using features related to article shares, such as self-reference shares and keyword metrics.

3. **Approach 3:**
   - Clustering after applying **PCA** to reduce the number of highly correlated features.

### How to Run the Notebook

1. Load the `OnlineNewsPopularity.csv` dataset.
2. Execute the notebook cells step by step to preprocess the data, perform clustering, and visualize the results.
3. Adjust clustering parameters such as the number of clusters and features used to explore different analysis perspectives.

### Output

The notebook outputs visualizations, including:

- 3D scatter plots of article clusters.
- Silhouette analysis plots showing the quality of clustering.
- Violin and bar plots showing the distribution of article shares across content categories and weekdays.

### Conclusion

This notebook provides an end-to-end analysis of the **Online News Popularity** dataset, combining clustering techniques with advanced visualizations to gain insights into article share patterns. You can customize the analysis further by experimenting with different clustering algorithms, features, and visualizations.

---

Feel free to explore and modify the code to suit your needs!
