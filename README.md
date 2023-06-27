# Customer_Segmentation_System

## Project Description:

The Customer Segmentation System is an application that uses k-means clustering to segment customers based on their annual income and spending score. The goal of this project is to group similar customers together to gain insights for targeted marketing strategies and personalized customer experiences.

**Technologies Used:**

1. Python: The programming language used to implement the project.
2. Google Colab: The platform used for running and executing the code.
3. Pandas: Used for data manipulation and analysis.
4. Matplotlib and Seaborn: Utilized for data visualization and creating plots.
5. Scikit-learn: The library used for implementing the k-means clustering algorithm.

## Steps of the Project:

**1. _Importing the necessary libraries and files:_**
  * The google.colab and files libraries are imported to handle file uploads in the Google Colab environment.
  * The numpy, pandas, matplotlib, seaborn, and sklearn.cluster libraries are imported for data analysis, visualization, and clustering.

**2. _Uploading and loading the dataset:_**
  * The files.upload() function is used to upload the Customers.csv file to Google Colab.
  * The pd.read_csv() function is used to load the dataset into a Pandas DataFrame.

**3. _Data exploration and preprocessing:_**
  * The head() function is used to display the first 5 rows of the dataset.
  * The shape attribute is used to determine the number of rows and columns in the dataset.
  * The info() function is used to obtain information about the dataset, such as the data types of columns and the presence of any missing values.
  * The isnull().sum() function is used to check for missing values in the dataset.

**4. _Feature selection and clustering:_**
  * The iloc function is used to select the columns representing the annual income and spending score.
  * The selected features are stored in the X variable as a NumPy array.
  * A loop is used to calculate the within-cluster sum of squares (WCSS) for different numbers of clusters.
  * The k-means clustering algorithm is applied to the data using the KMeans class from scikit-learn.
  * The labels for each data point are obtained using the fit_predict() method.

**5. _Elbow method and visualization:_**
  * The WCSS values for different numbers of clusters are stored in the wcss list.
  * A line plot is created using Matplotlib and Seaborn to visualize the WCSS values against the number of clusters.
  * The plot helps to identify the optimal number of clusters by locating the "elbow" point, which represents the point of diminishing returns in terms of WCSS reduction.

**6. _Clustering and visualization of results:_**
  * The k-means clustering algorithm is applied again with the chosen number of clusters.
  * The labels for each data point based on their clusters are stored in the Y variable.
  * A scatter plot is created to visualize the different clusters and their corresponding data points.
  * Each cluster is represented by a different color, and the centroids of the clusters are plotted as cyan markers.

The Customer Segmentation System utilizes k-means clustering to identify distinct customer groups based on their annual income and spending score. The project employs various libraries and tools to load the dataset, perform data analysis, implement the clustering algorithm, and visualize the results. The elbow method is utilized to determine the optimal number of clusters, and the final clusters are plotted on a scatter plot along with their centroids. This project helps businesses gain insights into customer behavior and tailor their marketing strategies accordingly.
