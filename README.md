# E-Commerce Data
This dataset consists of orders made in different countries from December 2010 to December 2011. The company is a UK-based online retailer that mainly sells unique all-occasion gifts. Many of its customers are wholesalers. 

Not sure where to begin? Scroll to the bottom to find challenges!



import pandas as pd

pd.read_csv("online_retail.csv")

## Data Dictionary
| Variable    | Explanation                                                                                                                       |
|-------------|-----------------------------------------------------------------------------------------------------------------------------------|
| InvoiceNo   | A 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c' it indicates a cancellation. |
| StockCode   | A 5-digit integral number uniquely assigned to each distinct product.                                                             |
| Description | Product (item) name                                                                                                               |
| Quantity    | The quantities of each product (item) per transaction                                                                             |
| InvoiceDate | The day and time when each transaction was generated                                                                              |
| UnitPrice   | Product price per unit in sterling (pound)                                                                                        |
| CustomerID  | A 5-digit integral number uniquely assigned to each customer                                                                      |
| Country     | The name of the country where each customer resides                                                                               |

[Source](https://archive.ics.uci.edu/ml/datasets/online+retail#)  of dataset.

**Citation:** Daqing Chen, Sai Liang Sain, and Kun Guo, Data mining for the online retail industry: A case study of RFM model-based customer segmentation using data mining, Journal of Database Marketing and Customer Strategy Management, Vol. 19, No. 3, pp. 197-208, 2012 (Published online before print: 27 August 2012. doi: 10.1057/dbm.2012.17).



## Don't know where to start?

**Challenges are brief tasks designed to help you practice specific skills:**

- 🗺️ **Explore**: Negative order quantities indicate returns. Which products have been returned the most?
- 📊 **Visualize**: Create a plot visualizing the profits earned from UK customers weekly, monthly, and quarterly.
- 🔎 **Analyze**: Are order sizes from countries outside the United Kingdom significantly larger than orders from inside the United Kingdom?

**Scenarios are broader questions to help you develop an end-to-end project for your portfolio:**

You are working for an online retailer. Currently, the retailer sells over 4000 unique products. To take inventory of the items, your manager has asked you whether you can group the products into a small number of categories. The categories should be similar in terms of price and quantity sold and any other characteristics you can extract from the data.

You will need to prepare a report that is accessible to a broad audience. It should outline your motivation, steps, findings, and conclusions.


## Exploratory Data Analysis
Data Preprocessing
We start by loading the dataset and performing data preprocessing tasks such as handling missing values, duplicates, and data inconsistencies. We also convert the InvoiceDate column to a proper datetime format to facilitate time-based analysis.

**Product Returns Analysis**
Negative order quantities in the dataset indicate product returns. We analyze which products have been returned the most, providing insights into potential issues with specific items and opportunities for improvement in quality control or customer satisfaction.

**Profit Visualization**
We visualize the profits earned from UK customers to identify any recurring patterns or seasonality. Line or bar plots are used to illustrate the weekly, monthly, and quarterly trends in profits, helping the retailer plan inventory and marketing strategies accordingly.

**Order Size Analysis**
To compare order sizes between the UK and non-UK countries, we conduct a statistical analysis. By examining the average order sizes, we determine if there is a significant difference in purchasing behavior between these customer segments.

## Conclusion
In this analysis of the E-commerce dataset, we explored various aspects of the data to derive actionable insights. We identified products with the highest return rates, allowing the retailer to focus on addressing potential quality or customer satisfaction issues. Additionally, we visualized the profits earned from UK customers on a weekly, monthly, and quarterly basis to understand seasonal trends and optimize inventory management.

Furthermore, we conducted an analysis to compare the order sizes between the UK and non-UK countries, providing insights into potential variations in customer behavior across regions. These findings can guide the retailer in tailoring marketing approaches and optimizing business strategies for different customer segments.

Overall, this EDA provides a foundation for data-driven decision-making and offers valuable information to enhance customer experience, increase profitability, and improve inventory management for the online retailer.

For a more detailed analysis, please refer to the Jupyter Notebook provided in this repository
