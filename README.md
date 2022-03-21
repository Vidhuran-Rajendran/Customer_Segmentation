# Customer-Segmentation
![image](https://user-images.githubusercontent.com/92842078/159161538-bb0bdd90-5bb5-44c1-9dcd-5924dc638c89.png)



# **Project Title** : Extraction/identification of major topics & themes discussed in news articles.
Problem Description
In this project, your task is to identify major customer segments on a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.
Data Description
Attribute Information:
### InvoiceNo: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation.
### StockCode: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
### Description: Product (item) name. Nominal.
### Quantity: The quantities of each product (item) per transaction. Numeric.
### InvoiceDate: Invice Date and time. Numeric, the day and time when each transaction was generated.
### UnitPrice: Unit price. Numeric, Product price per unit in sterling.
### CustomerID: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
### Country: Country name. Nominal, the name of the country where each customer resides.
Architecture
Data Preparation and Exploratory Data Analysis > Build Model using Multiple Techniques/Algorithms > Optimal Model identified through Testing and Evaluation



# **Summary**
First imported the libraries and dataset which was in excel file and This dataset contains 541909 rows and 8 columns, then checked for duplication of data and null values.

There were more than 120000 null values present in CustomerID Column it main column as other column was filled with zero and drop all values.

Various plots are visualized to see Outliers and Applied Inter Quartile Range method.

Data was used different units so its scaled using Standard Scaler and normalise data.

To find Number Clusters we applied Elbow Method and silhouette score the Selected Cluster Size with Visualized Graph.

K-Means Clustering was applied,

Dendrogram Linkage and Hierarchical Agglomerative Clustering Models are applied

# **Conclusion**
Given Data for Customer Segmentation most of them are irrelevant like StockCode, Description.etc and there is no relation.
After Applying Elbow and Silhouette score are more at cluster size =3 or 2
Same results applied with Dendrogram results of Kmeans Clusters Centers in plots appears better than Hierarchical Agglomerative Clustering

Cluster_0 CustomerID's take more time gap between Each Oder they Placed (Rarely).

Cluster_1 CustomerID's Makes always a Bulk Purchases which leads high Spending's (Retailers).
Cluster_2 CustomerID's Has Highest Orders Placed (Small Shops with less inventory).
