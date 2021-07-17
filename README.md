#Retail Customer Segmentation

In this project I analysed sales data from over over 500,000 transactions from an online store. I perform EDA on after cleaning the data and focus on customer metrics. I use K-means to cluster each customer into 4 categories and make recommendations on how to retain this category in the future.

# Dependencies

* python 3.8
* numpy
* pandas
* sklearn
* matplotlib
* mpl_toolkits
* seaborn
* pycountry
* plotly

# Analysis

* Most of the purchases and revenue occurs from August-November peaking in November.
* Compared the proportionate amount spent by each country (in £). UK sales accounted for approximately 82% of the total amount spent on the store. This is followed by countries in the EU, Australia and Japan.
* 8 of the top 10 customers with the highest number of invoices are from the UK. 

The average customer:
  * Has made their last purchase in the last 50 days
  * Spends £17.73 on their purchase
  * Buys 41 items in total, across all purchases

# K-means Clustering

Customers were segmented into equal sized bins of 600-1200 customers ber segment. These segments were categorised by the following:

  * **Cluster 0**: Low recency score, low frequency and monetary scores. These are not frequent customers. 
  * **Cluster 1**: High recency score, high frequency scores and low monetary scores. These are retained customers who make small, frequent purchases. 
  * **Cluster 2**: High scores in all categories. These are the preferred customers who are highly sought after. Targeted advertising for this group is suggested.
  * **Cluster 3**: Low recency score, low frequency score and high monetary score. These are customers who make one-off purchases on the site, generally for more expensive items.

# Recommendations

* Targeted advertising for customers characterising those in cluster 2 (i.e. have high RFM scores). 
* Send out randomised surveys within this group (cluster 2) or perform a/b testing to make their online shopping experience better.
* Start a customer loyalty program to better retain all groups
* Retain cluster 3 customers, perhaps by reducing prices for more expensive items. Could offer credit on next purchase.
* Target customers who buy from the UK
