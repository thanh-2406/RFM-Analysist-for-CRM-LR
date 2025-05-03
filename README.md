**Customer Churn Analysis and Segmentation using RFM and Machine Learning**

This repository contains a Python-based analysis pipeline for segmenting customers and predicting churn using RFM (Recency, Frequency, Monetary) analysis, KMeans clustering, and Decision Tree classification. The goal is to identify customer behavior trends and predict potential churn to inform targeted marketing strategies.

**Introduction to RFM Analysis**

RFM (Recency, Frequency, Monetary) is a marketing framework used to segment customers based on their purchasing behavior:





Recency (R): How recently a customer made a purchase. Lower recency (more recent purchases) is better.



Frequency (F): How often a customer makes purchases. Higher frequency indicates greater engagement.



Monetary (M): The total amount spent by a customer. Higher monetary value reflects greater contribution to revenue.

By scoring customers on these metrics, businesses can categorize them into segments (e.g., loyal, at-risk, new) and tailor strategies to improve retention and revenue.

**Problem Statement**

**1. Data Introduction**

The dataset, shopping_trends_2.csv, is used to analyze customer shopping behavior. It includes information on demographics, purchase transactions, payment methods, and seasonal consumption trends, providing a comprehensive view of customer interactions with the business.

**2. General Data Information**





Number of Records: 3,900



Number of Attributes: 21



Missing Values: None, ensuring a clean dataset for analysis.

**3. Key Attributes**





Customer Information:





Customer ID, Age, Gender, Salary (USD), Location



Transaction Information:





Item Purchased, Category, Purchase Amount (USD), Size, Color, Season



Shopping Behavior:





Subscription Status, Payment Method, Preferred Payment Method, Frequency of Purchases



Transaction & Promotion Details:





Shipping Type, Discount Applied, Promo Code Used, Previous Purchases



Transaction Timing:





Customer Time (Date of Purchase)

**4. Descriptive Statistics**





Age: Ranges from 18 to 70, with an average of approximately 44 years.



Popular Product Categories: Clothing, Footwear, Accessories, Electronics.



Average Spending: $59.76, with a range of $20 to $100.



Common Payment Methods: Credit Card, PayPal, Cash, Venmo, Bank Transfer.



Subscription Rate: 73% of customers are not subscribed to a membership program.



Average Salary: $90,097, ranging from $30,043 to $149,961.

**5. Consumer Trend Analysis**





Seasonal Spending: Highest in winter, lowest in summer, likely due to year-end holidays and discounts.



Age-Based Trends: Older customers tend to purchase more, possibly due to greater brand loyalty and financial stability.



Spending vs. Income: Spending is not strongly correlated with income, suggesting purchases are driven more by need or preference than salary.

Technologies Used





Python: Core programming language for data processing and analysis.



Pandas: For handling and manipulating tabular data (DataFrames).



NumPy: For numerical computations on arrays and matrices.



Matplotlib: For creating static visualizations like the Elbow plot.



Plotly: For interactive 3D visualizations of customer clusters.



Scikit-learn: For machine learning tasks, including:





MinMaxScaler (data normalization)



KMeans (clustering)



PCA (dimensionality reduction)



DecisionTreeClassifier (churn prediction)



Metrics (silhouette score, accuracy, classification report)



Google Colab: For running the analysis pipeline with Google Drive integration for data access.



Datetime: For processing date and time data in RFM calculations.
