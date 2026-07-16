#  customer-rfm-analysis-Project



An end-to-end *RFM (Recency, Frequency, Monetary) analysis* in Python — segmenting 1,000 customers based on real transaction behavior to identify Champions, Big Spenders, Recent, Frequent, and Lost customers, followed by a Pareto (80/20) revenue analysis.




##  Project Overview

| | |
|---|---|
| *Project Name* | Customer Segmentation using RFM Analysis |
| *Objective* | Segment customers by purchasing behavior and identify the most valuable customer groups |
| *Dataset* | Customer Master Data + Customer Transactions (1,000 customers, 23,050 transactions) |
| *Tools Used* | Python — Pandas, NumPy, Matplotlib (Jupyter / Google Colab) |
| *File Type* | Jupyter Notebook (.ipynb) |

---

##  Business Problem

A business with a large, growing customer base needs to know *who its most valuable customers are* — and who is at risk of churning — so it can prioritize retention and marketing spend. RFM analysis answers this by scoring every customer on how recently they bought, how often they buy, and how much they spend.

---

## 🗂️ Dataset

*Customer Master Data* — one row per customer (CustomerID, JoinDate, demographic fields)
*Customer Transactions* — one row per transaction (CustomerID, TransactionDate, TransactionAmount)

After cleaning, all *23,050 transaction records* contained valid `CustomerID`s that matched the customer master dataset, confirming full data consistency.

---

##  Project Workflow

### Step 1 — Load the Data
Loaded the Customer Master and Customer Transactions CSVs into Pandas DataFrames and previewed shape, structure, and data types.

### Step 2 — Clean the Data
- Converted JoinDate and TransactionDate to proper datetime format.
- Checked for and handled missing values (dropna).
- Validated CustomerID uniqueness in the master table and confirmed every transaction's CustomerID existed in the master dataset.

### Step 3 — Merge Datasets
Left-joined Customer_Transactions with Customer_Master_Data on CustomerID to build a single analysis-ready DataFrame.

### Step 4 — Calculate RFM Metrics
Using groupby('CustomerID'):
- *Recency* — days since each customer's most recent transaction
- *Frequency* — count of transactions per customer
- *Monetary* — total transaction amount per customer

### Step 5 — Score RFM
Used pd.qcut() to bucket each metric into quintiles, producing R_Score, F_Score, and M_Score (1–5 each).

### Step 6 — Build Combined RFM Segment
Concatenated the three scores into a single segment code (e.g., "555", "111").

### Step 7 — Assign Segment Labels
Applied business rules to translate segment codes into human-readable labels:

| Segment Code Pattern | Label |
|---|---|
| 555 | Champions |
| 111 | Lost |
| R = 5 (not 555) | Recent |
| F = 5 (not 555) | Frequent |
| M = 5 (not 555) | Big Spender |
| All other combinations | Others |

### Step 8 — Visualize & Analyze
- Bar chart of customer count per segment
- Pie chart of revenue contribution per segment
- Recency vs. Monetary scatter plot, colored by segment
- *Pareto analysis* — tested whether the top 20% of customers generate 80% of revenue

---

##  Key Insights

- *Largest segment:* "Others" (543 customers) — a broad group with average, non-extreme purchasing behavior.
- *Champions:* only 35 customers, but they show the highest recency, frequency, and spend — the most valuable and loyal segment.
- *Big Spenders:* 165 customers contribute *22.3% of total revenue*, making them a high-leverage segment despite their smaller size.
- *Recency vs. spend relationship:* customers who purchased more recently (0–30 days) tend to spend more, suggesting a negative relationship between recency and monetary value.
- *Pareto (80/20) rule does not hold:* the top 20% of customers do *not* generate 80% of revenue — revenue is more evenly spread across the customer base, meaning the business depends on a broad base rather than a small high-value group.

---

##  Skills Demonstrated

- Data cleaning, type conversion, and referential integrity validation across multiple datasets
- Multi-table merging with Pandas (pd.merge)
- RFM metric calculation using groupby, aggregation, and datetime arithmetic
- Quantile-based scoring (pd.qcut) and rule-based customer segmentation
- Data visualization: bar charts, pie charts, and multi-color scatter plots
- Pareto / cumulative revenue analysis

---

##  How to Use

1. Clone/download this repository.
2. Open python_Mini_Project.ipynb in Jupyter Notebook, JupyterLab, or Google Colab.
3. Update the file paths for Customer_Master_Data and Customer_Transactions CSVs to point to your local copies.
4. Run all cells sequentially — each step includes inline analysis insights.

---















This project is for learning and educational purposes.
