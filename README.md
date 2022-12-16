# Cryptocurrencies
#### Analysis by: Elaine Bermudez
  
## Project Overview
###  
A README.md that includes the purpose of the repository and short description of what was accomplished. Although there is no graded written analysis for this challenge, it is encouraged and good practice to add a brief description of your project.

You and Martha have done your research. You understand what unsupervised learning is used for, how to process data, how to cluster, how to reduce your dimensions, and how to reduce the principal components using PCA. It’s time to put all these skills to use by creating an analysis for your clients who are preparing to get into the cryptocurrency market.

Martha is a senior manager for the Advisory Services Team at Accountability Accounting, one of your most important clients. Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked you to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

The data Martha will be working with is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she has decided to use unsupervised learning. To group the cryptocurrencies, Martha decided on a clustering algorithm. She’ll use data visualizations to share her findings with the board.

The purpose of this project is to use unsupervised machine learning to analyze a database of cryptocurrencies and create a report including the traded cryptocurrencies classified by group according to their features.
This classification report could be used by an investment bank to propose a new cryptocurrency investment portfolio to its clients.
We use the following methods for the analysis:

- Preprocessing the database,
- Reducing the data dimension using Principal Component Analysis,
- Clustering cryptocurrencies using K-Means,
- Visualizing classification results with 2D and 3D scatter plots.

## Resources
- Data Source: crypto_data.csv
- Software: Jupyter Notebook 6.4.8, Python 3.7.13
- Library: Pandas, Scikit-learn library

## Results
<b>Elbow Curve</b>
- An elbow curve is created using hvPlot to find the best value for K.
- Predictions are made on the K clusters of the cryptocurrencies’ data

<img src="https://github.com/laneyberm/Cryptocurrencies/blob/main/Resources/images/elbow_curve.png" width="600">

<b>3D Scatterplot</b>
- The clusters are plotted using a 3D scatter plot, and each data point shows the CoinName and Algorithm on hover
- Precision is 0.99

<img src="https://github.com/laneyberm/Cryptocurrencies/blob/main/Resources/images/3D_scatterplot.png" width="600">

<b>Tradable cryptocurrencies</b>
- A table with tradable cryptocurrencies is created using the hvplot.table() function
- The total number of tradable cryptocurrencies is .

<img src="https://github.com/laneyberm/Cryptocurrencies/blob/main/Resources/images/tradables.png" width="600">

<b>2D Scatterplot</b>
- A hvplot scatter plot is created where the X-axis is "TotalCoinsMined", the Y-axis is "TotalCoinSupply", the data is ordered by "Class", and it shows the CoinName when you hover over the data point.
- Precision is 0.99

<img src="https://github.com/laneyberm/Cryptocurrencies/blob/main/Resources/images/2D_scatterplot.png" width="600">
  

## Summary and Recommendations
The table below is the summary results for all the Machine Learning (ML) models. The overall best ML model was the Easy Emsemble with AdaBoost Classifer. It's Balanced Accuracy Score is 0.9316, Precision is 1.00, Sensitivity is 1.00, and F1 is 1.00. In addition to the ML models, we ran a Model Tester with different parameters in n_estimators to see if ther are other conditions that would have a better Machine Learning model. But found that the Easy Ensemble AdaBoost Classifier was still the best recommendation to predict credit risk. 

