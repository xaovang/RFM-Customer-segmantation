RFM Customer Segmentation

This project uses SQL-based RFM analysis to segment customers based on their purchase behavior. The resulting dataset is exported as a .csv file and included in this repository.

---

What is RFM?

"RFM" stands for:

- Recency: How recently a customer made a purchase
- Frequency: How often they make purchases
- Monetary: How much money they spend

Each customer is scored from 1 to 5 in each category, where:
5 = most engaged/spending recently
1 = least engaged/spending

The scores are combined into an RFM_Score (555, 431, 211), and each customer is also labeled into a segment (Champion or Other).

---

Files Included

| File Name                   | Description                                |
|-----------------------------|--------------------------------------------|
|  rfm_results.csv            | Final RFM dataset with scores and segments |
|  README.md                  | Project overview and explanation           |
|  Amazon Sales Data Cleaned  | Amazon Sales Data                          |

---

Tools Used

- MySQL – Querying and calculating RFM scores
- SQL Window Functions – For Recency calculation using (DATEDIFF)
- GitHub – Dataset hosting and version control


Columns in rfm_results.csv

| Column            | Description                               |
|-------------------|-------------------------------------------|
|  customer_name    | Unique customer identifier                |
|  recency_score    | Score based on days since last purchase   |
|  frequency_score  | Score based on number of purchases        |
|  monetary_score   | Score based on total spending             |
|  rfm_score        | Combined score (e.g., 545)                |
|  customer_segment | Segment label (Champion or Other)         |

---

Example Use Cases

- Identify top customers to reward with loyalty programs
- Target inactive customers with re-engagement campaigns
- Prioritize marketing spend based on customer lifetime value

---

Data Source

Kaggle: Amazon Sales Dataset: (https://www.kaggle.com/datasets/zahidmughal2343/amazon-sales-2025)

