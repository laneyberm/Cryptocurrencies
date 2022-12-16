# Cryptocurrencies
#### Analysis by: Elaine Bermudez
  
## Project Overview
###  
The Advisory Services Team at Accountability Accounting is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked us to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

We are using unsupervised learning to process data, to cluster, to reduce your dimensions, to reduce the principal components using PCA and a clustering algorithm to group the cryptocurrencies. We will create a report including the traded cryptocurrencies classified by group according to their features. We use the following methods for the analysis:

- Preprocessing the database,
- Reducing the data dimension using Principal Component Analysis,
- Clustering cryptocurrencies using K-Means,
- Visualizing classification results with 2D and 3D scatter plots.

## Resources
- Data Source: crypto_data.csv
- Software: Jupyter Notebook 6.4.8, Python 3.7.13
- Library: Pandas, Scikit-learn library

## Results
<b>Clustering Cryptocurrencies using K-Means - Elbow Curve</b>
- An elbow curve is created using hvPlot to find the best value for K.
- The best k value appears to be 4 so we would conclude on an output of 4 clusters to categorize the crytocurrencies.

<img src="https://github.com/laneyberm/Cryptocurrencies/blob/main/Resources/images/elbow_curve.png" width="600">

<b>3D Scatterplot</b>
- Using the PCA algorithm to reduce the crytocurrencies dimensions to three principal components, the clusters are plotted using a 3D scatter plot, and each data point shows the CoinName and Algorithm on hover. 

<img src="https://github.com/laneyberm/Cryptocurrencies/blob/main/Resources/images/3D_scatterplot.png" width="600">

<b>Tradable cryptocurrencies</b>
- The total number of tradable cryptocurrencies is 532.

<img src="https://github.com/laneyberm/Cryptocurrencies/blob/main/Resources/images/tradables.png" width="600">

<b>2D Scatterplot with TotalCoinMined vs TotalCoinSupply</b>
- A hvplot scatter plot is created where the X-axis is "TotalCoinsMined", the Y-axis is "TotalCoinSupply", the data is ordered by "Class", and it shows the CoinName when you hover over the data point.

<img src="https://github.com/laneyberm/Cryptocurrencies/blob/main/Resources/images/2D_scatterplot.png" width="600">
  

## Summary and Recommendations
We have identified the classification of 532 cryptocurrencies based on similarities of their features.

<b>Recommendation:</b>
Particularities of each group need to be analyzed to determined their performance and potential interest for the investment bank's clients.

