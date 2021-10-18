# Cryptocurrencies

## Overview 

In this challenge we use unsupervised learning to help us make sense of cryptocurrencies.

Unsupervised learning is used when we don't yet know the question we're asking of the data. When we just want to figure out if there is anything at all the data can tell us. 
It can be best explained by the below image

![Machine-Learning-Explained2](https://user-images.githubusercontent.com/85518330/137792456-b57a504a-1765-40fb-9e82-77db4c6961be.png)

## Resources

Software: Jupyter Notebooks

Languages: Python

Libraries: numpy, pandas, scikit-learn, plotly, Pyviz hvplot, 

Data Sources: Cryptocurrencies Data: crypto_data.csv

## Project Objectives & Methodology 

Like they say the quality of our output will largely depend on the quality of our input data. Hence it is very critical that we examine and prepare our data well before we decide to run any models on it. Below is the stepwise process we followed  

* **Data Selection** - crypto_data.csv - A prelimnary check on the data to find out 

  * How many columns/rows it has, 
  
  * How many nulls,
  
  * What are the data types of the columns 
  
  * What information is contained in them, 
  
  * What data can be removed?


* **Data Processing** - For data processing, the focus is on making sure the data is set up for the unsupervised learning model, which requires the following:
   
    *  Null values are handled. 
    
    *  Only numerical data is used. 
    
    *  Values are scaled. In other words, data has been manipulated to ensure that the variance between the numbers won't skew results.

* **Data Transformation** This step involves transforming the data into a convenient way for others to use in the future.

* **Data Clustering** Clustering is a type of unsupervised learning that groups data points together 
    
    *  K-means Algorithm
      
        * Initialize the K starting centroids

        * Assign datapoints to the nearest centroid

        * Group datapoints

        * Visualize the data
    
    *  Hierachical 
       
       Also known as agglomerative clustering, works with groups (clusters) of data points. The algorithm starts by declaring each point with its own cluster, then merges the        two most similar clusters until a declared stopping point has been reached

* **Trial & Error & Elbow Curves** 
  In most instances of unsupervised learning models the number of clusters is not known and it is arrived at by trial and error or by using the **elbow curve**. To create an   elbow curve, we'll plot the clusters on the x-axis and the values of a selected objective function on the y-axis.
  
* **Dimensionality Reduction** 
  The process of reducing features is called dimensionality reduction - Feature elimination & Feature extraction
    
* **Principal Component Analysis**
  PCA is a statistical technique to speed up machine learning algorithms when the number of input features (or dimensions) is too high. PCA reduces the number of dimensions     by transforming a large set of variables into a smaller one that contains most of the information in the original large set.

## Results

Our Crytocurrencies data gave us the following results

Using the elbow curve method we found out that the ideal number of clusters is 4

<img width="575" alt="elbow_curve" src="https://user-images.githubusercontent.com/85518330/137804416-9af907fc-f4e8-4cb2-bb7f-ec273a914764.png">

Our 3D Scatter plot was a shown below

<img width="712" alt="3D_scatter_plot" src="https://user-images.githubusercontent.com/85518330/137804498-b4c7e03a-1993-41d1-aee9-b91ce156ab63.png">

The scatter plot of totalCoinsMined vs TotalCoinsSupply was as shown below

<img width="576" alt="Scatter_plot" src="https://user-images.githubusercontent.com/85518330/137804637-e33ec888-7b71-490c-970d-d3beac9e5a0d.png">
