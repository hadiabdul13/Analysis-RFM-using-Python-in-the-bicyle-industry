## Creator Profile:
Abdul Hadi - [hadiabdul13@gmail.com](hadiabdul13@gmail.com) | [LinkedIn](https://www.linkedin.com/in/abdul-hadi-447608159/)

# Optimizing Marketing Budget Efficiency in the Bicycle Industry through RFM Analysis in Python

## Introduction  
In the bicycle industry, an effective marketing strategy is not just about how much is spent but how efficiently the budget is allocated. One of the main challenges is ensuring that marketing funds are directed toward customers with long-term profit potential while minimizing waste on less responsive segments. A data-driven approach is essential to achieve efficiency and maximize impact.

## RFM Analysis for Customer Segmentation  
To optimize marketing efforts, Recency, Frequency, and Monetary (RFM) Analysis is used to segment customers based on their purchasing behavior:  

- **Recency (R):** How recently a customer made their last transaction.  
- **Frequency (F):** How often a customer makes transactions within a given period.  
- **Monetary (M):** How much a customer has spent in total.  

Using RFM segmentation, businesses can identify high-value customers for loyalty programs, target inactive customers with re-engagement strategies, and exclude low-value customers from expensive marketing campaigns. This enables efficient resource allocation, enhancing the effectiveness of marketing campaigns while minimizing budget waste.

## Data Source  
The dataset used in this analysis consists of bicycle sales transactions from a company in 2017. It contains 19,445 transactions from 3,492 customers. The dataset includes key attributes such as transaction date, customer ID, product details, and total spending. This dataset can be downloaded [here](https://drive.google.com/file/d/1CYYyWQaAZxi7DWi05WGqV5XGcD_uH_1L/view?usp=drive_link).

## Exploratory Data Analysis (EDA)  
Before performing RFM segmentation, EDA was conducted to clean and preprocess the dataset. The following steps were taken:  
- Handling missing values: Columns such as *Online Order*, *Brand*, and *Product Size* had missing values, which were removed.  
- Checking duplicates: No duplicate records were found.  
- Descriptive statistics: The average transaction value is $1,107 (*SD* = $583), with a minimum of $12 and a maximum of $2,091.

## RFM Calculation  
Each customer’s Recency, Frequency, and Monetary values were computed using the following formulas:  

- **Recency (R):** Number of days since the last transaction. **(R = {Current Date} - {Last Transaction Date})**
- **Frequency (F):** Total number of transactions per customer. **{Count of Transactions per Customer}**
- **Monetary (M):** Total spending per customer. **M = {Transaction Value per Customer}**

## Summary of RFM Metrics  
- **Recency:** Customers had an average recency of 62.85 days (*SD* = 59.37), with values ranging from 0 to 353 days.  
- **Frequency:** Customers made an average of 5.52 transactions (*SD* = 2.28), ranging from 1 to 14 transactions.  
- **Monetary:** The average total spending per customer was $6,113 (*SD* = $2,898), with a range from $60 to $19,071.

## Customer Segmentation Based on RFM  
Customers were segmented into three groups based on their Recency and FM Score (Frequency + Monetary Score):

| **Segment**   | **Recency Score** | **FM Score** | **Description** |
|--------------|-----------------|------------|----------------|
| **VIP**      | ≥ 3             | ≥ 3        | High-value customers with frequent purchases and high spending |
| **Loyal**    | ≥ 2             | ≥ 2        | Regular buyers with consistent engagement |
| **General**  | Otherwise       | Otherwise  | Low-value customers needing re-engagement |

## Marketing Budget Efficiency with Segmentation  

Without segmentation, all customers receive equal marketing efforts, leading to higher costs. Assuming *X* represents the marketing budget per customer, the total marketing cost without segmentation is:

**{Total Cost} = (1598 + 1023 + 869) \times 1.25X = 5273.75X**

### **Optimized Marketing Budget with Segmentation**  
With segmentation, the marketing budget is strategically distributed as follows:  
- **VIP Customers:** High-priority marketing with a budget of 1.1X per customer.  
- **Loyal Customers:** Moderate effort with 1.2X per customer.  
- **General Customers:** Cost-effective promotions with 1.3X per customer.  

The new optimized marketing cost is:

**{Marketing Cost} = (1598 \times 1.1X) + (1023 \times 1.2X) + (869 \times 1.3X) = 4874.1X**

### **Cost Savings with RFM Segmentation**  
By implementing targeted marketing, segmentation leads to a 7.58% reduction in total marketing costs, ensuring that resources are allocated efficiently while improving customer retention and revenue growth.

## Conclusion  
By applying RFM Analysis, businesses in the bicycle industry can:  
- Identify and reward high-value customers (VIPs).
- Optimize marketing efforts for Loyal customers.  
- Minimize budget waste on low-value customers. 
- Reduce overall marketing costs by 7.58%.
- Maximize ROI through data-driven strategies.  

*"Data-driven segmentation is the key to marketing efficiency—by understanding customer value, businesses can allocate resources strategically, reduce unnecessary costs, and maximize return on investment."*  
