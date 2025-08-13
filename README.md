# 🛍️ Customer Segmentation using K-means Clustering

This project utilizes the K-means clustering algorithm to segment customers based on their Annual Income and Spending Score. Customer segmentation is a crucial technique for businesses to understand their customer base better and tailor marketing strategies effectively.

## **📊 Dataset**

The dataset used for this project is Mall_Customers.csv. It contains the following columns:

* **CustomerID**: Unique identifier for each customer.
* **Gender**: Gender of the customer (Male/Female).
* **Age**: Age of the customer.
* **Annual Income (k$)**: Customer's annual income in thousands of dollars.
* **Spending Score (1-100)**: A score assigned by the mall based on customer behavior and spending habits.

## **✨ Features**

* **Data Loading and Initial Exploration**: Loads the Mall_Customers.csv dataset into a pandas DataFrame and performs initial checks like viewing the first few rows (.head()), checking the dimensions (.shape), and getting a summary of data types and non-null values (.info()).

* **Missing Value Check**: Confirms the absence of missing values in the dataset.

* **Feature Selection**: Selects 'Annual Income (k$)' and 'Spending Score (1-100)' as the features for clustering, as these are key indicators of customer spending behavior.

* **Elbow Method for Optimal Clusters**: Implements the Elbow Method to determine the optimal number of clusters (k) for the K-means algorithm. This is visualized through an Elbow Point Graph showing the WCSS (Within-Cluster Sum of Squares) for different numbers of clusters.

* **K-means Model Training**: Trains the K-means clustering model with the identified optimal number of clusters (in this case, 5 clusters as suggested by the Elbow Method).

* **Cluster Assignment**: Assigns a cluster label to each data point (customer) based on their proximity to the cluster centroids.

* **Cluster Visualization**: Plots all the clusters and their respective centroids using a scatter plot. Each cluster is represented by a different color, and centroids are distinctly marked, making it easy to visualize the customer groups.

## **🛠️ Technologies Used**

* **Python**

* **pandas**: For data manipulation and analysis.

* **numpy**: For numerical operations.

* **matplotlib.pyplot**: For creating static visualizations, especially the Elbow Method plot and cluster visualization.

* **seaborn**: For enhanced statistical data visualizations and plotting the Elbow Method graph.

* **scikit-learn**: For machine learning functionalities, specifically KMeans for clustering.

## **📦 Requirements**

To run this project, you will need the following Python libraries:

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn

## **🚀 Getting Started**

To get this project up and running on your local machine, follow these simple steps.

### **Installation**

1. **Clone the repository (if applicable):**

```
git clone <repository_url>
cd <repository_name>
```

2. **Install the required Python packages:**

```
pip install pandas numpy matplotlib seaborn scikit-learn
```

### **Usage**

1. **Place the dataset**: Ensure the Mall_Customers.csv file is located in the same directory as the Jupyter notebook (Customer Segmentation using K-means Clustering.ipynb).

2. **Run the Jupyter Notebook**: Open and execute all the cells in the Customer Segmentation using K-means Clustering.ipynb notebook in a Jupyter environment (e.g., Jupyter Lab, Jupyter Notebook, Google Colab).

The notebook will:

* Load and inspect the customer data.
* Apply the Elbow Method to find the optimal number of clusters.
* Train the K-means model and assign clusters.
* Generate a scatter plot visualizing the different customer segments and their centroids.

## **📈 Results**

The project successfully segments customers into distinct groups based on their annual income and spending score. The Elbow Method helps in identifying the most appropriate number of clusters, which in this case leads to 5 meaningful customer groups. The visualization clearly shows these groups, enabling businesses to understand different customer behaviors and target them with personalized strategies.

## **🧑‍💻 Contributing**

Contributions are welcome! If you have suggestions for improvements, new features, or bug fixes, please feel free to:

1. Fork the repository.
2. Create your feature branch (git checkout -b feature/your-feature-name).
3. Make your changes.
4. Commit your changes (git commit -m 'Add new feature').
5. Push to the branch (git push origin feature/your-feature-name).
6. Open a Pull Request.

## **📄 License**

This project is open-source and available under the MIT License.
