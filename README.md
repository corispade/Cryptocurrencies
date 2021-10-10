# Cryptocurrencies

# Overview

Using unsupervised machine learning to create an analysis on a dataset of cryptocurrencies and discover trends for clients who are preparing to get into the cryptocurrency market. We are creating a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for new investment. 

## Process:

View code [here](https://github.com/corispade/Cryptocurrencies/blob/main/crypto_clustering.ipynb) for reference of the below deliverables.

### Deliverable 1: Using Pandas to preprocess and clean the data set
* Keep all cryptocurrencies that are currently being traded
* Remove rows with at least one null value
* Filtering to only keep rows where coins have been mined
* Remove columns that will not be used in clustering algorithm
* Use get_dummies() to create variables for the text features
* Use StandardScaler fit_transform() function to standardize the features

### Deliverable 2: Reducing Data Dimensions using PCA
* Apply PCA to reduce dimensions to three principal components
* Create a new DataFrame from the three principal compnenents to run the analysis

### Deliverable 3: Clustering Cryptocurrencies Using K-Means
* Create an elbow curve using hvPlot to find the best value for K
* Run the K-Means algorithm to make predictions of the K clusters for cryptocurrencies data
* Create a new DataFrame adding the coin data, principal components and class (predictions)

### Deliverable 4: Visualizing Cryptocurrencies Results
* Create 3D scatter plot using Plotly Express scatter_3d() function
* Create table with tradable cryptocurrencies using hvplot.table()
* Use MinMaxScaler().fit_transform() method to scale the coin supply and coins mined columns
* Create a new dataframe with coin supply, coins mined, and class (predictions)
* Create hvplot scatter plot to visualize coin supply and coins mined data

## Resources:
Data Source: [crypto_data.csv](https://github.com/corispade/Cryptocurrencies/blob/main/Resources/crypto_data.csv)

Software: Python 3.7.6, Conda 4.10.1

Environment: Jupyter Notebook

Dependencies: Pandas, Scikit-Learn, Plotly


# Results:

### Deliverable 1: 

Preprocessed DataFrame for PCA analysis:

![image](https://github.com/corispade/Cryptocurrencies/blob/main/Images/D1_Cleaned_DF.png)

### Deliverable 2: 

DataFrame presenting three principal components for K-means analysis:

![image](https://github.com/corispade/Cryptocurrencies/blob/main/Images/D2_PCA_DF.png)

### Deliverable 3: 

Elbow curve informed from PCA analysis:

![image](https://github.com/corispade/Cryptocurrencies/blob/main/Images/D3_Elbow_Curve.png)

Cleaned DataFrame with class predictions for visualization:

![image](https://github.com/corispade/Cryptocurrencies/blob/main/Images/D3_Combined_DF.png)

### Deliverable 4: 

3D scatter plot to visualize the four clusters:

![image](https://github.com/corispade/Cryptocurrencies/blob/main/Images/D4_3D_Plot.png)

Table of tradable cryptocurrencies:

![image](https://github.com/corispade/Cryptocurrencies/blob/main/Images/D4_Tradable_Table.png)

Scatter plot showing Total Coin Supply and Total Coins Mined by Class:

![image](https://github.com/corispade/Cryptocurrencies/blob/main/Images/D4_Scatter.png)

