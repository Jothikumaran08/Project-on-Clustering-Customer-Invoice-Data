# Project-on-Clustering-Customer-Invoice-Data
This project focuses on clustering customer invoice data to identify distinct customer segments based on their purchasing behavior. By grouping customers with similar characteristics, businesses can tailor marketing strategies, improve customer engagement, and enhance sales performance.


Dataset Description

The dataset contains the following key features:

CustomerID: Unique identifier for each customer.

InvoiceDate: Date of each invoice.

Quantity: Number of items purchased.

UnitPrice: Price per item.

Country: Customer's country of origin.

New features derived for analysis include:

Total_Bill_Size: Total purchase amount for each customer.

First_Purchase: Date of the customer's first purchase.

Last_Purchase: Date of the customer's most recent purchase.

Most_Common_Location: Country where the customer most frequently shops.

Top_Item: The most frequently purchased item by each customer.

Purchase_Interval_Days: Number of days between the first and last purchase.

Data Cleaning Explanation

To ensure data quality, the following steps were performed:

Converted InvoiceDate to datetime format for easier manipulation.

Added calculated features like Total_Bill_Size and Purchase_Interval_Days for deeper insights.

Standardized the Total_Bill_Size column using StandardScaler for improved clustering performance.

Clustering Analysis

The KMeans algorithm was applied to the standardized Total_Bill_Size feature with 3 clusters.

Each customer was assigned to one of these clusters, indicating their purchasing pattern.

Visualizations for Key Insights

1. Distribution of Total Bill Size

A histogram showing the distribution of total bill sizes to identify common spending patterns.

2. Customer Segmentation Visualization

A scatter plot showcasing customer clusters based on total bill size, providing insights into distinct customer groups.

3. Correlation Heatmap

A heatmap highlighting relationships between key features to uncover potential dependencies.

Instructions for Running the Project

Clone the repository:

git clone <repository_link>
cd Project_on_clustering_customer_invoice_data

Install the required libraries:

pip install -r requirements.txt

Run the Jupyter Notebook:

jupyter notebook notebooks/Project_on_clustering_customer_invoice_data.ipynb

Follow the instructions within the notebook for data analysis and visualization.

Required Libraries (requirements.txt)

pandas
numpy
matplotlib
seaborn
scikit-learn

