#  customer-rfm-analysis-python

> End-to-end customer analytics project focused on customer segmentation, RFM analysis, revenue analysis, and business insight generation using Python.

The dataset contains:

- Customer Master Data
- Customer Transaction Data
- Jupyter Notebook Files
- Project Report
---

# 📌 Project Overview

This project focuses on analyzing customer purchasing behavior using **RFM (Recency, Frequency, Monetary) Analysis** and customer segmentation techniques.

This project performs Customer Segmentation using the RFM (Recency, Frequency, Monetary) model. The analysis helps businesses identify their most valuable customers, understand purchasing behavior, and create targeted marketing strategies.

The project uses customer master data and transaction data to calculate RFM metrics and categorize customers into different segments.

---

## Objectives

- Clean and validate customer and transaction datasets
- Merge customer and transaction information
- Calculate RFM metrics:
  - Recency
  - Frequency
  - Monetary Value
- Generate RFM scores using quantile-based ranking
- Create customer segments
- Visualize customer distribution and revenue contribution
- Perform Pareto Analysis on customer revenue

---

# 🚀 Business Problem

Businesses often face challenges in:
- Identifying their most valuable customers
- Understanding customer purchasing behavior
- Detecting inactive or churn-risk customers
- Improving retention strategies
- Increasing revenue through targeted marketing

This project solves these business problems through customer segmentation and data-driven analysis.

---

# 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

# 📂 Dataset Information

The project uses two datasets:

## 1️⃣ Customer Master Dataset
Contains customer demographic details such as:
- CustomerID
- Name
- Gender
- Age
- City
- Marital Status
- Number of Children
- Join Date

## 2️⃣ Customer Transactions Dataset
Contains:
- CustomerID
- Transaction Date
- Transaction Amount

---

# 📊 Dataset Highlights

- Total Customers: **1,000**
- Total Transactions: **23,050**
- Customer-centric transaction analysis
- Revenue-based purchasing behavior analysis

---

# ⚙️ Project Workflow

## ✅ Data Loading
- Imported datasets using Pandas
- Checked dataset structure and datatypes
- Previewed customer and transaction records

---

## ✅ Data Cleaning & Preprocessing

Performed:
- Datatype conversion
- Missing value detection
- Duplicate validation
- CustomerID consistency validation
- Date formatting
- Dataset merging

The datasets were cleaned and validated successfully without major inconsistencies.

---

## ✅ RFM Analysis

### RFM Metrics Used

### 🔹 Recency (R)
Days since the customer's last purchase.

### 🔹 Frequency (F)
Total number of purchases made by the customer.

### 🔹 Monetary (M)
Total amount spent by the customer.

---

## ✅ RFM Scoring

Customers were scored using quantile-based segmentation:
- R Score → 1 to 5
- F Score → 1 to 5
- M Score → 1 to 5

Combined RFM scores were then used to classify customer behavior.

---

# 👥 Customer Segmentation

Customers were segmented into:
|----------|-------------|
| Champions | Most valuable customers |
| Big Spender | High spending customers |
| Frequent | Customers who purchase often |
| Recent | Recently active customers |
| Lost | Inactive customers |
| Others | Average customers |

---

# 📈 Key Insights from the Analysis

## 🔹 Champion Customers
Only **35 customers** were categorized as **Champions**, but they generated very high transaction value with strong recent engagement and frequent purchasing behavior.

These customers represent the most valuable segment of the business.

---

## 🔹 Big Spender Insight
The **Big Spender** segment consisted of approximately **165 customers** contributing a significantly high share of total business revenue.

This indicates that a smaller group of customers drives premium sales performance.

---

## 🔹 Revenue Concentration Insight
The top **20% of customers contributed approximately 27% of total revenue**, indicating that revenue distribution is more balanced and does not strictly follow the traditional Pareto 80/20 principle.

---

## 🔹 Lost Customer Insight
Around **34 customers** were identified as **Lost Customers**, showing:
- Low purchase activity
- Lower spending behavior
- High recency values

These customers represent potential churn risks for the business.

---

## 🔹 Spending Pattern Insight
Customers with:
- Lower recency values
- Higher transaction frequency

generally demonstrated significantly higher monetary contribution.

This shows a strong relationship between customer engagement and revenue generation.

---

## 🔹 Revenue Distribution Insight
The analysis showed that revenue generation is distributed across multiple customer segments instead of depending heavily on only a few customers.

This suggests:
- Better revenue stability
- Reduced dependency risk
- Balanced customer contribution

---

# 📊 Visualizations Created

The project includes:
- Customer Segment Distribution Chart
- Revenue Contribution  Pie Chart
- Recency vs Monetary Scatter Plot
- Pareto Analysis Chart
- Segment-wise Revenue Distribution Graphs

---

## Key Insights

- Champions represent the most loyal and valuable customers.
- Big Spenders contribute a significant share of revenue.
- Recent customers show strong engagement potential.
- Lost customers may require re-engagement campaigns.
- Revenue is distributed across a broad customer base rather than following the traditional 80/20 Pareto rule.


# 📌 Business Recommendations

## ✅ Retain Champion Customers
- Loyalty programs
- Premium rewards
- Exclusive access offers

---

## ✅ Re-engage Lost Customers
- Personalized email campaigns
- Discount offers
- Customer win-back strategies

---

## ✅ Increase Customer Frequency
- Cross-selling
- Product recommendations
- Repeat purchase incentives

---

## ✅ Focus on High Monetary Customers
- VIP benefits
- Personalized communication
- Premium customer experience

---

## Future Improvements

- Advanced customer lifetime value prediction
- Machine learning-based segmentation
- Interactive dashboards using Power BI or Tableau
- Automated marketing recommendations
  

```

## Author

Trishula Mitra

## License

This project is for learning and educational purposes.
