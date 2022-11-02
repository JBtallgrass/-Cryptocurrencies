# Cryptocurrencies

## Background
Advisory Services Team at Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked for a  report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.
## Purpose
The data is not ideal, so it is processed to fit the machine learning models. Since there is no known output the team has decided to use unsupervised learning. To group the cryptocurrencies, the project uses a clustering algorithm. The attached data visualizations illustrate the findings.

## Deliverables
This project consists of four technical analysis deliverables. 

### Deliverable 1: Preprocessing the Data for PCA

All cryptocurrencies that are not being traded were removed in additon to the IsTrading column being dropped. All null values, all columns without coins being mined 

A new DataFrame is created that stores all cryptocurrency names from the CoinName column and retains the index from the crypto_df DataFrame (5 pt)
The get_dummies() method is used to create variables for the text features, which are then stored in a new DataFrame, X (5 pt)
The features from the X DataFrame have been standardized using the StandardScaler fit_transform() function (5 pt)

### Deliverable 2: Reducing Data Dimensions Using PCA

### Deliverable 3: Clustering Cryptocurrencies Using K-means

### Deliverable 4: Visualizing Cryptocurrencies Results

![3-D scatter plot](https://github.com/JBtallgrass/-Cryptocurrencies/blob/main/Images/3D_ScatterPlot.png)
![3-D scatter plot](https://github.com/JBtallgrass/-Cryptocurrencies/blob/main/Images/Elbow_plot.png)
![Bokeh plot](https://github.com/JBtallgrass/-Cryptocurrencies/blob/main/Images/bokeh_plot.png)
