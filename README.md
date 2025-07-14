# Customer-Segmentation-using-K-Means-Clustering
Project Overview

This project demonstrates the application of K-Means Clustering, a fundamental unsupervised learning algorithm, to perform customer segmentation. The goal is to identify distinct groups or segments of customers within a dataset based on their annual income and spending behavior at a mall.

By understanding these segments, a business can develop targeted marketing strategies, improve customer relationships, and make informed decisions. This project showcases a complete workflow from data exploration to identifying and interpreting the final customer clusters.

Dataset 📊

The project utilizes the "Mall Customer Segmentation Data" from Kaggle, which is an ideal dataset for clustering tasks.

    Source: Mall Customer Segmentation Data on Kaggle

    File Used: Mall_Customers.csv

    Key Features Used:

        Annual Income (k$): The annual income of the customer.

        Spending Score (1-100): A score assigned by the mall based on customer behavior and spending nature.

Project Workflow ⚙️

The project follows a structured methodology to discover and analyze customer segments:

    Data Loading and Exploration: The Mall_Customers.csv dataset is loaded and an initial Exploratory Data Analysis (EDA) is performed to understand its structure and check for any missing data.

    Feature Selection and Scaling:

        The two most relevant features for this segmentation task, Annual Income (k$) and Spending Score (1-100), are selected.

        These features are then scaled using StandardScaler. This is a critical step because K-Means is a distance-based algorithm and requires features to be on a comparable scale.

    Finding the Optimal Number of Clusters (The Elbow Method):

        To determine the best number of clusters (k) for the data, the Elbow Method is employed.

        This involves running the K-Means algorithm for a range of k values (1 to 10) and plotting the Within-Cluster Sum of Squares (WCSS) for each.

        The "elbow" point on the plot, where the rate of decrease in WCSS sharply changes, indicates the optimal k. For this dataset, k=5 was identified as the optimal number.

    Model Training:

        A KMeans model is trained on the scaled data with the optimal number of clusters (k=5).

        The model assigns each customer to one of the five clusters.

    Visualization and Interpretation of Clusters:

        The results are visualized using a scatter plot, where each point represents a customer, colored according to their assigned cluster.

        The centroids (centers) of each cluster are also plotted. This visualization provides a clear view of the distinct customer segments.

Technologies Used 💻

    Python 3

    Pandas (for data manipulation)

    NumPy (for numerical operations)

    Scikit-learn (for K-Means clustering and preprocessing)

    Matplotlib & Seaborn (for data visualization)

    Jupyter Notebook / Google Colab

How to Run This Project ▶️

    Download Files:

        Obtain the project notebook (.ipynb file).

        Download the Mall_Customers.csv dataset from the Kaggle link provided above.

    Setup Environment:

        Open the notebook file in Google Colab or a local Jupyter Notebook instance.

        Upload the Mall_Customers.csv file to the same environment.

    Execute Code:

        Run the notebook cells sequentially from top to bottom to replicate the entire analysis and clustering process.

Results and Conclusion 💡

The K-Means algorithm successfully segmented the customers into five distinct groups based on their income and spending scores. These segments can be interpreted for business strategy:

    Careful Spenders: High income, but low spending score.

    Standard Customers: Average income and average spending.

    Target Audience: High income and high spending score (ideal customers).

    Sensible Spenders: Low income and low spending score.

    Potential Customers: Low income, but high spending score.

This segmentation provides valuable business intelligence, allowing the mall to tailor marketing campaigns, promotions, and services to each specific customer group.
