# Customer Churn Analysis

A complete customer churn analysis project — from raw SQL data to a machine learning model that predicts which customers are likely to churn.

##  Project Overview
This project analyzes subscription-based customer data to understand churn behavior and predict future churn risk. Data was extracted from a SQLite database, cleaned, merged, and analyzed to uncover key business insights.

##  Process
- Extracted data from a SQLite database (customer, subscription, and support tables) using Python
- Cleaned messy real-world data — fixed column names, standardized categories, handled missing values, corrected date formats
- Merged three tables into a single analysis-ready dataset
- Engineered features: churn flag, customer tenure, customer age, complaint count, churn risk tier
- Performed exploratory data analysis: churn by plan type, state, and subscription type
- Built a correlation heatmap to find drivers of churn
- Trained a Random Forest Classifier to predict churn probability per customer
- Visualized results using Matplotlib and Seaborn

##  Key Findings
- Overall churn rate: **28.57%** (Retention rate: 71.43%)
- Basic plan customers churn at **60%**, vs. only **14.3%** for Premium plan users
- Referral-acquired customers churn the most (**83.3%**) compared to Organic (0%) and Paid (16.7%)
- Support escalations are strongly correlated with churn (**correlation: 0.77**)
- Average customer tenure: ~1535 days

## Tech Stack
- Python (pandas, numpy)
- SQLite3
- Matplotlib, Seaborn
- scikit-learn (Random Forest Classifier)

##  How to Run
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Open `churn_analysis.ipynb` in Jupyter Notebook or VS Code
4. Run all cells

##  Files
- `churn_analysis.ipynb` — full analysis notebook
- `requirements.txt` — required Python libraries