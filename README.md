# E-commerce Customer Segmentation Using Unsupervised Learning

Project Overview:

This project focuses on segmenting customers from an e-commerce platform using unsupervised learning techniques. By analyzing customer transactional behavior and demographic data, the goal is to create meaningful customer groups. These segments will be used to tailor marketing strategies and offer personalized coupons, enhancing customer loyalty and satisfaction.

Objectives:

1.Segment customers based on demographic features (e.g., gender, city) and transactional behavior (e.g., coupon usage, transaction frequency).
2.Analyze the segmented groups and provide insights on customer behavior patterns.
3.Identify customer groups that share similar behaviors.
4.Develop recommendations for offering targeted coupons to maximize loyalty and satisfaction.

Dataset:

The dataset consists of the following tables:
1.Customers: Basic demographic information (e.g., customer ID, gender, city).
2.Transactions: Details of coupon transactions (e.g., claimed, burnt).
3.Cities: Information about the cities associated with customers.
4.Branches: Details about merchant branches.
5.Merchants: Information on merchants.

Methods Used

1.Data Preprocessing:
-Data from multiple tables to create a unified dataset are merged, which included demographic and transactional features.
-Features such as the number of transactions, number of burnt coupons, and time difference between transactions were extracted.
-We performed feature scaling using StandardScaler to ensure that features like transaction count and coupon usage are properly scaled.

2. Clustering Algorithm:
-The K-Means applied clustering algorithm to segment the customers into different groups.
-The optimal number of clusters was chosen using the Elbow Method, which identifies the point at which the rate of improvement in clustering decreases.
-The Silhouette Score was calculated to evaluate the quality of the clustering.

3. Cluster Analysis:
After applying the K-Means algorithm, we analyzed each cluster based on:
Frequency of coupon usage
Number of transactions
Demographics (gender, city)

Implementation:

Python: The entire project is implemented in Python.
Libraries Used:
pandas for data manipulation.
scikit-learn for clustering algorithms and model evaluation.
matplotlib for visualizing the results.

Steps:

1.Load and Merge Data: Combined customer, transaction, gender, and city data to form a single dataset.
2.Feature Engineering: Extracted features like transaction frequency, coupon usage, and demographic data.
3.K-Means Clustering: Trained a K-Means model to segment the customers into distinct groups.
4.Evaluation: Used Silhouette Score to assess the quality of the clustering.
5.Visualization: Created scatter plots to visualize customer groups based on transactional behavior
6.Cluster Analysis: Each cluster was analyzed to understand customer behavior patterns, such as frequency of coupon usage and demographics.

Results:

3 distinct customer segments were identified:
Frequent Users: Customers who regularly burn coupons and have high transaction frequency.
Occasional Users: Customers who claim coupons but rarely burn them.
Inactive Users: Customers with low interaction in terms of both claiming and burning coupons.

Recommendations:

1.Frequent Users: Offer exclusive deals and loyalty programs to keep them engaged.
2.Occasional Users: Encourage more frequent coupon burns through reminders and limited-time offers.
3.Inactive Users: Re-engage these customers with personalized discounts or "welcome back" offers.

Conclusion:

This project demonstrates the power of unsupervised learning to segment customers and derive actionable insights. The results help businesses understand customer behavior and offer personalized incentives to enhance customer satisfaction and loyalty.

