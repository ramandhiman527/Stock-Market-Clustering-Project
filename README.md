# Stock-Market-Clustering-Project
This machine learning project is about clustering similar companies with K-means clustering algorithm. The similarity is based on daily stock movements.

## Intro
A dictionary ‘companies_dict’ is defined where 'key' is company's name and 'value' is company's stock code. 25 companies are considered.
Stock market data is extracted from yahoo finance.
The stock movement of companies would be compared based on these 6 parameters :- 'High', 'Low', 'Open', 'Close', 'Volume', 'Adj Close'.

'movement' is defined as difference of opening and closing prices of a particular day.
Positive movement suggests to go long on stock (buy) and negative movement suggests to short the stock(sell).

## VISUALIZING THE DATA :
'Movement' as defined earlier is difference of closing and opening prices of a particular day.
The variation of 'movement' of companies (amazon, apple) in the time period from 2015–01–01 to 2017–02–01 is plotted.

## Need of Normailzation
Stock prices of some companies have different scales. The goal of Normalization is to change the value of numeric columns in the dataset to a common scale without distorting differences in the range of values.

## CREATING A PIPELINE
Now we create a pipeline that normalizes the data and then applies K-Means clustering algorithm to cluster companies with similar daily stock movements.

## PCA Reduction
The high dimensional data ‘norm_movement’ with 755 features(755 days) is reduced to a 2 dimensional data with 2 features(2days) and then k-means clustering is applied.

cons of PCA : some details are lost. The results are not very accurate.
