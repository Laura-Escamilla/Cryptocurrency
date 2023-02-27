# Cryptocurrency

## Project Overview

For this project we used our knowledge of unsupervised learning, how to process data, how to cluster, how to reduce your dimensions, and how to reduce the principal components using PCA. All of this with the purpose to create an analysis for the client Accountability Accounting, a prominent investment bank, that is interested in offering a new cryptocurrency investment portfolio for its customers.

So we created a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

## Results

The data we worked with were not ideal so we had to processed to fit the machine learning models. Since there is no known output for what the client is looking for, we decided to use unsupervised learning. To group the cryptocurrencies, we opted on a clustering algorithm. And data visualizations will be used to share the findings with the board of the bank.

Here we have the data before the preprocessing for PCA:

<img width="343" alt="Preprocessed_Data" src="https://user-images.githubusercontent.com/113747210/221665084-f70da3e6-6e4a-4deb-9503-24ecea6a954a.png">

We keeped all the cryptocurrencies that are being traded:

<img width="347" alt="Keep_traded" src="https://user-images.githubusercontent.com/113747210/221665521-f6a020dc-df73-445a-b3ac-e8da28d91224.png">

Keeped the rows where coins are mined:

<img width="356" alt="Coins_mined" src="https://user-images.githubusercontent.com/113747210/221666359-8f6d86bf-01a5-414d-a7ae-caba0b2a160f.png">

We created a DataFrame with the three principal components:

<img width="355" alt="DataFrame_3PC" src="https://user-images.githubusercontent.com/113747210/221666761-e47c0a07-50ee-4d8f-b5bb-4cacb5b7fbd7.png">

We created an elbow curve to find the best value for K, initialize K-Means model, fit the model and predict clusters:

<img width="360" alt="Elbow_curve_K" src="https://user-images.githubusercontent.com/113747210/221667348-87595ab4-a2e5-4c21-9b54-1c3196e28c8d.png">

Now we have a DataFrame that includes predicted clusters and cryptocurrencies features. We concatenated the crypto data and the pcs data, added the coin name column that holds the names of crytocurrencies and a "class" column that holds the predictions.

<img width="431" alt="DataFrame2" src="https://user-images.githubusercontent.com/113747210/221668403-f2600021-8d7c-4b49-90dd-0084f20f8cad.png">

Finally we have the viusalizing cryptocurrencies results:

<img width="442" alt="3d" src="https://user-images.githubusercontent.com/113747210/221669125-fc0982a2-9d7c-43ff-b650-5b9110be1af2.png">

<img width="442" alt="table" src="https://user-images.githubusercontent.com/113747210/221669405-7503a862-e685-42af-ae56-850b83d1e6b1.png">

<img width="442" alt="scatter" src="https://user-images.githubusercontent.com/113747210/221669769-80c27af5-aad7-4708-83a4-9f5b624aab16.png">

