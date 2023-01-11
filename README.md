# Cryptocurrencies
- Unsupervised learning model is different from supervised learning in that an unsupervised model provides unlabeled data that the algorithm understands by extracting features and patterns on its own. 
- In a supervised leaning model, the algorithm learns on a labeled dataset, and helps predict outcomes for unforeseen data. 
- In other words, supervised learning is used when we know what we are looking for or what the output should be. Unsupervised learning is used when we don’t know the question we are asking the data.

## Overview of the project:
- In this project, we used unsupervised learning for, how to process data, how to clustered the data, how to reduce dataframe dimensions, and how to reduce the principle components using PCA. 
- Through the use of this knowledge, we will create an analysis for a client who is preparing to get into the cryptocurrency market.

## Results:

- The data that is initially given is not ideal so first we processed to fit the machine learning models. Since there is no known output, unsupervised learning was used. To look at the difference cryptocurrencies, it was decided to use a clustering algorithm.

- Python was used as the tool for this analysis and divided into four parts: Processing the Data for PCA (Principal component Analysis), reducing the data dimensions using PCA, clustering cryptocurrencies using K-means, and finally visualizing cryptocurrencies results.

- The first visualization that was made was through the use of and elbow curve to determine the number of cluster which is used in Kmeans algorithm:

!()[]

- Created a 3D scatter plot using the Plotly Express scatter_3d() function to plot the three clusters from the clustered_df DataFrame.

!()[]

- Created a table with tradable cryptocurrencies using the hvplot.table() function.

!()[]

- Lastly, the MinMaxScaler().fit_transform method used to scale the TotalCoinSupply and TotalCoinsMined columns between the given range of zero and one. After that Create a new Dataframe using clustred dataframe.
- plot an hvplot scatter plot with x="TotalCoinsMined", y="TotalCoinSupply", and by="Class", and  it shows the CoinName when you hover over the data point.

!()[]