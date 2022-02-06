# Cryptocurrency_Clusters
Unsupervised Machine Learning


## Background 
Created a report that includes what cryptocurrencies are on the trading market. Determined whether they can be grouped to create a classification system for this new investment.

Processed data to fit t-SNE & k-Means.

## Steps
### Data Preparation

* Read `crypto_data.csv` into Pandas. The dataset was obtained from [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist).

* Discard all cryptocurrencies that are not being traded. 
* Remove all rows that have at least one null value.
* Filter for cryptocurrencies that have been mined.
* Covert dataset to numeric be comprehensible to a machine learning algorithm.
* Use Pandas to create dummy variables for `Algorithm` and `ProofType`, into numerical data. 
* Standardize the dataset so that columns that contain larger values do not unduly influence the outcome.

### Dimensionality Reduction

* Performed dimensionality reduction with PCA. Preserved 90% of the explained variance in dimensionality reduction.

* Further reduced the dataset dimensions with t-SNE and visually inspect the results.

### Cluster Analysis with k-Means

* Create an elbow plot to identify the best number of clusters. 
* Determine the inertia for each `k` between 1 through 10 to identify the number of the clusters

### Recommendation

* Based on the visualization and analysis above, this cryptocurrencies dataset can be clustered into 4 distinct groups. I would recommand my clients at the investment bank that the cryptocurrencies can be grouped and created a classification system in order to develop a new investment portfolio for their customers.