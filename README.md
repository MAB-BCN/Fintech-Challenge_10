In this Challenge, we analyzed the price change data of a group of cryptocurrencies in different periods.
After normalizing the data with StandardScaler and creating a dataframe, we used the elblow method to find the best value for k. Below is the plot of the resulting Elbow Curve:

https://github.com/MAB-BCN/Fintech-Challenge_10/blob/main/Elbow_curve_originaldata.PNG

We then used the K-means model to cluster the cryptocurrencies using the original data, and created a scatter plot using hbPlot that included a new column with the predicted clusters. Below is a picture of the resulting scatter plot:

https://github.com/MAB-BCN/Fintech-Challenge_10/blob/main/Scatter_plot_originaldata.PNG

We then created a PCA model to reduce the 3 principal components and retrieve the explained variance to determine the percentage of information that could be attributed to each component, resulting in .>92%

After creating a new dataframe with the new PCA data, we then applied the same methods as with the original data: Elbow Method and Clustering, as shown in the following pictures:

https://github.com/MAB-BCN/Fintech-Challenge_10/blob/main/Elbow_curve_pcadata.PNG
https://github.com/MAB-BCN/Fintech-Challenge_10/blob/main/Scatter_plot_pcadata.PNG

After visually analyzing the cluster analysis results, we determined that the impact of using fewer features to cluster the data using K-Means results in clusters being more clearly defined, which is helpful as a starting point to analyze each cluster