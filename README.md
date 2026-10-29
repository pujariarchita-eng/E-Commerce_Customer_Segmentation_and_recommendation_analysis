# E-Commerce Customer Segmentation and Recommendation Analysis

## Project Overview
This project focuses on understanding customer purchasing behaviour using data analysis and machine learning. K-Means clustering is used to group customers based on their purchasing patterns, and a basic recommendation system suggests similar products based on previous transactions.

## Objectives
- Clean and prepare the online retail transaction dataset.
- Create customer-level Recency, Frequency and Monetary (RFM) features.
- Apply feature scaling and K-Means clustering.
- Use the elbow method to study the number of clusters.
- Visualize customer groups and understand their purchasing behaviour.
- Recommend similar products using cosine similarity.

## Dataset
**Dataset:** UCI Online Retail

The dataset contains transactions from a UK-based online retail business between December 2010 and December 2011.

Dataset link: https://archive.ics.uci.edu/dataset/352/online+retail

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- SciPy
- Jupyter Notebook

## Methodology

### 1. Data Cleaning
Removed duplicate records, missing customer details, cancelled invoices, returned quantities and invalid prices.

### 2. RFM Analysis
Created three features for each customer:
- **Recency:** Number of days since the customer's last purchase.
- **Frequency:** Number of distinct invoices.
- **Monetary:** Total amount spent by the customer.

### 3. Customer Segmentation
Applied StandardScaler and K-Means clustering to group customers. The elbow method was used to examine different cluster counts.

The four customer groups were labelled:
- Champions
- Regular Customers
- Occasional Buyers
- At-Risk Customers

### 4. Visualization
Created an elbow graph, a two-dimensional customer cluster visualization and a chart showing the number of customers in each segment.

### 5. Product Recommendation
Used cosine similarity on customer-product purchase data to recommend products with similar purchasing patterns.

## Results
The analysis identified four customer segments.

| Customer Segment | Number of Customers |
|---|---:|
| Champions | 571 |
| Regular Customers | 1,452 |
| Occasional Buyers | 1,377 |
| At-Risk Customers | 938 |

Champions had the highest average purchase frequency and spending among the four groups. The results can help businesses understand customer value and plan more targeted marketing activities.

## Files Generated
- `customer_segments.csv` — customer-level RFM features and cluster labels.
- `segment_summary.csv` — summary statistics for each customer segment.
- `cleaned_retail_transactions.csv` — cleaned transaction records with segment labels.

## How to Run the Project
1. Install Python and Jupyter Notebook.
2. Install the required libraries if they are not already installed.
3. Download the Online Retail dataset from the UCI repository.
4. Place `Online Retail.xlsx` in the same folder as the notebook.
5. Open `E-Commerce_Customer_Segmentation_and_recommendation_analysis.ipynb`.
6. Run the code cell and review the output graphs, tables and generated CSV files.

## Conclusion
This project helped me understand how customer transaction data can be used for segmentation and product recommendations. K-Means clustering helped identify groups with different purchasing behaviours, while cosine similarity provided a simple way to recommend related products.

The project demonstrates the use of Python, data preprocessing, unsupervised machine learning and basic recommendation techniques in an e-commerce application.

## Author
Completed as part of the Veda Technology internship project.
