# Cryptocurrencies


## Challenge Overview

### Purpose:

   The purpose of this analysis is to use unsupervised machine learning techniques is used for, preprocessing the data for PCA, reducing data dimensions using PCA, 
clustering cryptocurrencies using K-means, and visualizing cryptocurrencies results.   
  
 
## Resources
- Software:
   - Jupyter Notebook 6.4.6
   - Machine Learning
      - Python 
         - scikit-learn library
   
- Data source: 
   - [crypto_data.csv](https://github.com/SYDsCorner/Cryptocurrencies/blob/main/Resources/crypto_data.csv)
   
   
## Results 

### Deliverable 1: Preprocessing the Data for PCA


- **Preprocessing the Data**
   - Keep all the cryptocurrencies that are being traded
   - Keep all the cryptocurrencies that have a working algorithm
   - Remove unnecessary features
   - Remove null values
   - Keep the rows where coins are mined
   - Create a new DataFrame that holds only the cryptocurrencies names for using later
   
   - Drop the 'CoinName' column since it's not going to be used on the clustering algorithm
   ![1](https://user-images.githubusercontent.com/89308251/147378534-24d99c63-ecca-486c-8af5-7dc44f0fe1ae.jpg)
   
   - Use get_dummies() to create variables for text features
   - Standardize the data with StandardScaler()

### Deliverable 2: Reducing Data Dimensions Using PCA

![2](https://user-images.githubusercontent.com/89308251/147378810-f4b7b8e6-43ba-41ce-92cc-11bee6609db1.jpg)

- **Reducing Data Dimensions**
   - Use PCA to reduce dimension to three principal components
   - Create a DataFrame with the three principal components
 
### Deliverable 3: Clustering Cryptocurrencies Using K-means

- **Clustering Cryptocurrencies**
   - Create an **elbow curve** to find the best value for K
   ![3](https://user-images.githubusercontent.com/89308251/147378831-b1b531e2-88d7-4e07-9703-a5666ca2c81f.jpg)
   
   - Initialize the K-Means model, Fit the model, Predict clusters
   - Create a new DataFrame including predicted clusters and cryptocurrencies features

### Deliverable 4: Visualizing Cryptocurrencies Results 

- **Visualizing Cryptocurrencies**
   - Create a **3D-Scatter** with the PCA data and the clusters
   ![4 1](https://user-images.githubusercontent.com/89308251/147378865-0833652b-6379-4548-aa55-8b4a4debf139.jpg)
   
   - Create a table with tradable cryptocurrencies
      - There are ***532 tradable cryptocurrencies**
   ![4 2](https://user-images.githubusercontent.com/89308251/147378876-4220d4d1-de8b-495e-9b04-08506c22423f.jpg)
   
   - Scale the data to create the scatter plot with tradable cryptocurrencies
   - Create a new DataFrame that has the scaled data
   - Create a **2D-Scatter** 
   ![4 3](https://user-images.githubusercontent.com/89308251/147378894-bb695bbe-e82f-4fee-b0d1-be21f1ec8a32.png)


