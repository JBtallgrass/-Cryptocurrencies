# Cryptocurrencies

## Background
Advisory Services Team at Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked for a  report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.
## Purpose
The data is not ideal, so it is processed to fit the machine learning models. Since there is no known output the team has decided to use unsupervised learning. To group the cryptocurrencies, the project uses a clustering algorithm. The attached data visualizations illustrate the findings.

## Deliverables
This project consists of four technical analysis deliverables. 

### Deliverable 1: Preprocessing the Data for PCA

All cryptocurrencies that are not being traded were removed in additon to the *IsTrading* column being dropped. All null values, all columns without coins being mined, and the *Coinsmined* column are dropped. A new DataFrame was created storing all cryptocurrency names from the *CoinName* column and retains the index from the crypto_df DataFrame. The *get_dummies()* method creates variables for the text features, which are then stored in a new DataFrame, X which are features standardized using the StandardScaler fit_transform() function.

### Deliverable 2: Reducing Data Dimensions Using PCA
In deliverable #2 the PCA algorithm reduces the dimensions of the X DataFrame down to three principal components. The pcs_df DataFrame  has the following three columns, PC 1, PC 2, and PC 3, and has the index from the crypto_df DataFrame.

### Deliverable 3: Clustering Cryptocurrencies Using K-means
The K-means algorithm is used to cluster the cryptocurrencies using the PCA data, where the following steps have been completed:
An elbow curve is created using hvPlot to find the best value for K 
![Elbow plot](https://github.com/JBtallgrass/-Cryptocurrencies/blob/main/Images/Elbow_plot.png)

Predictions are made on the K clusters of the cryptocurrencies’ data and a new DataFrame is created with the same index as the crypto_df DataFrame and has the following columns: Algorithm, ProofType, TotalCoinsMined, TotalCoinSupply, PC 1, PC 2, PC 3, CoinName, and Class (5 pt)

### Deliverable 4: Visualizing Cryptocurrencies Results

![3-D scatter plot](https://github.com/JBtallgrass/-Cryptocurrencies/blob/main/Images/3D_ScatterPlot.png)

![Bokeh plot](https://github.com/JBtallgrass/-Cryptocurrencies/blob/main/Images/bokeh_plot.png)
