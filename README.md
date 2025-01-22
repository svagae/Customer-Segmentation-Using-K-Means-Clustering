# Customer Segmentation Using K-Means Clustering

## Description

This project aims to perform customer segmentation based on their annual income and spending score. Using the **K-means clustering** algorithm, the customers are grouped into clusters based on similarities in these two attributes. The goal is to identify distinct customer segments that can be used for targeted marketing and personalized offers.

### Dataset

The dataset used is the "Mall_Customers.csv," which contains customer data such as:

- **CustomerID**: Unique identifier for each customer.
- **Genre**: Gender of the customer.
- **Age**: Age of the customer.
- **Annual Income**: The annual income of the customer.
- **Spending Score**: A score assigned to customers based on their spending behavior.

### Tools and Libraries Used

- **Python**: Programming language.
- **Pandas**: Data manipulation and analysis.
- **NumPy**: Handling arrays and numerical operations.
- **Matplotlib**: Visualization of results.
- **Seaborn**: Advanced visualization library.
- **Scikit-learn**: Implementation of the K-means clustering algorithm.

## Installation

### Prerequisites

Make sure you have Python and the necessary libraries installed. You can install the required packages using `pip`:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Steps to Run

1. Clone or download the project files.
2. Ensure the dataset `Mall_Customers.csv` is in the correct directory (or adjust the path to where the dataset is stored).
3. Run the script in your preferred IDE or terminal.

```bash
# Run the script
python main.py
```

## Process Overview

1. **Data Loading**: The dataset is loaded using `pandas.read_csv()`.
2. **Data Preprocessing**: Check for missing values, and select the relevant columns (`Annual Income` and `Spending Score`) for clustering.
3. **Elbow Method**: Determine the optimal number of clusters (K) using the **Elbow method** based on the WCSS (Within-Cluster Sum of Squares).
4. **K-Means Clustering**: Apply the K-means algorithm to cluster the customers into 5 distinct groups.
5. **Visualization**: Plot the customer segments and visualize the centroids for each cluster.

## Results

- The **Elbow plot** shows the WCSS for different values of K, helping determine the optimal number of clusters.
- The **scatter plot** shows the five distinct customer groups with their corresponding centroids.
- Each group is represented by a different color, and the centroids are marked with a cyan dot.

## Visualizations

- **Elbow Method Plot**: Displays the WCSS for clusters ranging from 1 to 10, helping us identify the "elbow point" and the optimal number of clusters.
  
    

- **Customer Segments**: A scatter plot showing customer segments based on their annual income and spending score. Each cluster is represented by a different color, and the centroids are marked.

    

## Future Improvements

- **Use More Features**: Additional features such as age or gender could be included to improve the clustering and customer segmentation.
- **Cluster Interpretation**: Provide more detailed interpretation of each customer segment (e.g., targeting strategies based on income and spending score).
- **Advanced Clustering Techniques**: Experiment with other clustering algorithms like DBSCAN or Hierarchical clustering for comparison.

## Contributing

Feel free to fork the repository, report issues, or submit pull requests. Contributions to improve the model or add new features are always welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
