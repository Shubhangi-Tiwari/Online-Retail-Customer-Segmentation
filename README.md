#Capstone-Project- Unsupervised- Online Retail Customer Segmentation

Introduction
Provided with transnational data set which contains all the transactions, the main objective is to identify major customer segments.

Problem Statement
Online Retail Customer Segmentation

In this project, your task is to identify major customer segments on a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

Dataset Information
The provided Dataset is of transnational which consists detail of all the transactions occurred between 01/12/2010 and 09/12/2011. There are total 541909 rows and 8 columns in the provided dataset. In this dataset there are details for transaction including CustomerID, StockID, Description, InvoiceDate, InvoiceNo, Quantity, UnitPrice and Country. The main objective is to identify major customer segments for the same data set. Following are the details of all columns present:

InvoiceNo - Invoice number for the transaction.

StockCode - StockCode is the code for product.

Description - Description of the product.

Quantity - The quantities of each product per transaction.

InvoiceDate - Date of the Invoice.

UnitPrice - Product Price for each unit.

CustomerID - CustomerID uniquely assigned to each customer.

Country- The name of the country from where each customer resides. 

Data Preprocessing and Visualization

Data preprocessing involves cleaning and transformation data into suitable form for analysis. Data pre-processing involves Data Cleaning, Transformation and Data Reduction. Data Cleaning mainly removes any unwanted or null values, any missing data or noisy data is removed in cleaning. After cleaning data transformation is formed using Normalization techniques. Later Data reduction takes place when as per requirement particular column is created or any other unwanted column is removed using dimensionality reduction or any other method. This all steps are very important before implementing any model. Data visualization, in general makes complex data easy to understand and get significant insights from that entire dataset, so we used visualization which gave lots of insights of dataset, many questions were answered using graphs and visual plots. The graphs and visual plots used in this project are as follows:

Distribution plot
Bar plot
Pair Plot
Point Plot
Scatter Plot
Coorelation Heatmap
For this visualization mainly seaborn & matplotlib library were used.

Model Implementation

For Customer Segmentation, I have created a RFM (Recency,Frequency and Monetary) model which helps us understand when was the last time user purchased item? How frequently customer shops, and how much money did the customer spends. Depending on there factors a RFM model is build, accordingly RFM score and values are calculated. Depending on those scores segmentation is done. For model implementation used K Means Clustering with elbow and silhouette method, later Hierarchical Clustering is used, both these models help to find optimal number of clusters.

Conclusion

The conclusion drawn after entire data cleaning, processing, analysing, visualizing and implementing different machine learning models are as follows:

**Conclusion drawn after Data Analysis and Visualization are:**

1.The provided dataset is of transnational transactions of a non-store online retail with lots of null and duplicate values.

2.Top 5 products based on maximum selling are White Hanging Heart T-Light Holder followed by Regency Cakestand 3 Tier , Jumbo Bag Red Retrospot, Party Bunting and Lunch Bag Red Retrospot

3.Top 5 countries based on maximum number of customers are United Kingdom, Germany, France, EIRE and Spain.

4.Top 5 countries based on least number of customers are Lithuania followed by Brazil, Czech Republic Country, Bahrin and Saudi Arania.

5.Top five Customer IDs were found to be 12748 followed by 13089,13263,14096 & 14298

6.Top 5 StockCode of product are 85123A followed by 22423,85099B,84879 and 47566.

7.Created new variables such as Day,Month,year,month_num,day_name,hour and minute using InvoiceDate column.

8.Most of the customers purchased the items in month of November, December, September and October whereas least itesm were purchased in month of April, January and February.

9.Most of the purchases were made in between 10 AM to 2 PM whereas least purchase were made at 6 AM.

10.Found out total price for each order using Quantity and UnitPrice and created a new feature named as total_price.

**Conclusion drawn after Model Implementation:**

Created RFM model (Recency, frequency, monetary) which is used to identify a company's or an organization's best customers by using certain measures.

On the basis of RFM model, customers are segmented into groups, score of RFM individually and together decides in which group customer belongs.

After creating RFM model, Machine Learning Algorithm such as K Means Clustering and Hierarchical Clustering were implemented.

In K Means Clustering, used two methods named as Elbow Method and Silhouette Score Method to find the optimal number of clusters.

Hierarchical Clustering was also implemented which basically groups similar objects into groups called clusters represented in a hierarchy graph shown as a dendrogram.



