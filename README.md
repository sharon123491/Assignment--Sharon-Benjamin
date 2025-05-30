# 1Pay Data Analyst Assignment

## Project Overview

This project is part of a data analyst hiring assignment for 1Pay, a digital payments and wallet platform. The goal is to explore user behavior, transaction patterns, and fraud risks using the provided datasets. The analysis was performed entirely in Python using **Jupyter Notebook**, with visualizations generated via **pandas**, **matplotlib**, and **seaborn**.

---

## Files Included

- `1pay_analysis.ipynb`: Jupyter Notebook containing all analysis and code.
- `unified_dataset.csv`: Merged dataset combining users, transactions, and merchants.
- `README.md`: This instruction file.
- `Assignment Report`: PDF with graphs and business recommendations.

  How to Run the Notebook

###  Requirements
- Jupyter Notebook
- Python 3.x
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `datetime`

### Instructions

1. **Download the Datasets**  
   Place the following CSV files in your local **Downloads folder**:
   - `transactions.csv`
   - `users.csv`
   - `merchants.csv`

2. **Open the Notebook**  
   Launch Jupyter Notebook and open `1pay_analysis.ipynb`.

3. **Run the Notebook Section by Section**  
   Execute each code block **sequentially** to:
   - Load and inspect the data
   - Create a unified dataset
   - Perform exploratory data analysis
   - Apply rule-based fraud detection
   - Generate graphs and insights
  
   - Analysis Summary

### 1. **Transaction Trends**
- From **Nov 2024 to Mar 2025**, both transaction volume and value grew significantly.
- March 2025 marked the **peak**, with a slight decline in April–May, yet still higher than the baseline.
- Visualized using both **Power BI** and **Python (Seaborn)**.

### 2. **Conversion Rates by Transaction Type**
| Type   | Success Rate |
|--------|--------------|
| Wallet | 86.7%        |
| Card   | 85.9%        |
| UPI    | 85.7%        |

- All modes showed strong performance.
- Wallet slightly leads in conversion efficiency.

### 3. **Top 5 Spending Industries**
- Highest spending in: **Electronics**, followed by **Food**, **Retail**, **Health**, **Education**.
- Visuals generated using both Power BI and pandas.

### 4. **State-level Insights**
- **Tamil Nadu** has the highest number of active users and the highest average ticket size.
- Active = users with at least one successful transaction.

---

## Fraud Detection Heuristics

Rule-based logic was applied to flag potentially suspicious transactions:

1. **High-Value + Unverified KYC**
   - Users with KYC not verified and txns > ₹4,000

2. **Sudden Transaction Spikes**
   - 5+ transactions within 10 minutes by the same user

3. **Repeated Failed Attempts**
   - 3 or more failed txns within 5 minutes

> All fraud detection rules were implemented in **Python using pandas**, with SQL pseudocode included for reference.

---

## Business Recommendations

-  **Retain Users in Active States**: Focus loyalty programs in Delhi, TN, Gujarat
-  **Promote Wallet/UPI**: Higher conversion rates → more incentives
-  **Industry Tie-Ups**: Electronics merchants show highest spend
-  **Enforce KYC Tiers**: Incentivize verification + cap unverified txns

---

## Contact

Prepared by: **Sharon Benjamin**  
Email: *shrnbnjmn@gmail.com*  
