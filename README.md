
---

# 📊 Customer Shopping Behavior Analytics

**Python • SQL • Statistical Analysis • Power BI**

An end-to-end **customer analytics case study** analyzing retail shopping behavior to identify revenue drivers, evaluate subscription impact, and simulate business strategies using Python, SQL, and Power BI.

---

# 🚀 Project Overview

This project analyzes **3,900+ customer transactions** to understand customer behavior, purchasing patterns, and revenue distribution.

The analysis goes beyond descriptive dashboards by incorporating:

* **behavioral feature engineering**
* **customer segmentation**
* **statistical experimentation (A/B testing simulation)**
* **Pareto revenue analysis**
* **business scenario simulation**

The goal is to demonstrate **how data can support real business decisions in an e-commerce environment.**

---

# 🧩 Business Problem

Retail platforms often struggle to answer questions such as:

* Which customer segments drive the most revenue?
* Do subscription programs increase spending?
* Is revenue concentrated among a small group of customers?
* How would revenue change if subscription adoption increased?

This project investigates these questions using transactional shopping data to generate **data-driven business insights.**

---

# 📦 Project Workflow

The project follows a typical **data analytics lifecycle**.

## 1️⃣ Data Cleaning & Preparation (Python)

Raw customer transaction data was cleaned and transformed using **Pandas**.

Key steps included:

* Handling missing values using **category-level median imputation**
* Standardizing column naming conventions
* Creating engineered features such as:

  * `age_group`
  * `purchase_frequency_days`
  * `avg_order_value`
  * `customer_ltv_proxy`
  * `purchases_per_year`
* Loading processed data into **MySQL** for analysis

These features allow deeper behavioral analysis of customer spending patterns.

---

## 2️⃣ Database Analysis (SQL – MySQL)

SQL was used to perform business-focused analytics, including:

* Revenue distribution by **gender and age group**
* **Top-rated and most purchased products**
* **Shipping type impact on spending**
* **Customer segmentation** (New, Returning, Loyal)
* Discount usage patterns
* Product performance ranking using **window functions**
* Subscription behavior among repeat customers

---

## 3️⃣ Behavioral Analytics (Python)

Several analytical techniques were applied to better understand customer value.

### Customer Value Metrics

Engineered behavioral metrics such as:

* **Average Order Value (AOV)**
* **Customer Lifetime Value proxy**
* **Purchase frequency per year**

These metrics help estimate long-term customer contribution.

---

### Customer Value Segmentation

Customers were segmented into:

* **Low Value**
* **Medium Value**
* **High Value**

using quantile-based segmentation (`pd.qcut`) to compare spending patterns across groups.

---

### Pareto Revenue Analysis

A Pareto analysis evaluated revenue concentration.

Result:

> The top **20% of customers generate ~31% of total revenue**, indicating that revenue is relatively distributed across the customer base rather than concentrated among a small group of high-value users.

---

### A/B Testing Simulation

A statistical test was performed to evaluate whether **subscribers spend more than non-subscribers**.

A **two-sample t-test** compared purchase amounts between the two groups.

Result:

```
p-value = 0.662
```

This indicates **no statistically significant difference in spending behavior** between subscribers and non-subscribers.

---

### Revenue Impact Simulation

A business scenario simulation estimated how revenue might change if **subscription adoption increased**.

Scenario tested:

* Current subscription rate: **27%**
* Simulated rate: **40%**

Result:

> Revenue change was minimal (−0.08%), suggesting subscription programs may influence **customer engagement or retention rather than immediate spending.**

---

## 4️⃣ Visualization & Dashboard (Power BI)

An interactive **Power BI dashboard** was built to explore the data visually.

Dashboard features:

* Customer and revenue KPIs
* Sales distribution by category
* Age-group revenue analysis
* Subscription behavior
* Filters for shipping type, gender, and product categories

---

# 🔍 Key Insights

Major findings from the analysis include:

* Revenue is **relatively evenly distributed across age groups**, with young adults contributing the largest share (~26%).
* Customer spending patterns are **similar between subscribers and non-subscribers**.
* Revenue is **not highly concentrated**, indicating broad customer participation.
* Certain product categories (e.g., **Clothing and Accessories**) dominate sales volume.
* Discount usage plays an important role in product purchases.

---

# 💡 Business Recommendations

Based on the analysis:

**Improve subscription value**

Subscription programs should emphasize **loyalty benefits, retention, and convenience** rather than focusing solely on increasing spending.

**Optimize marketing strategy**

Target multiple customer segments rather than relying on a single demographic group.

**Promote high-performing categories**

Clothing and accessory products drive strong engagement and should be prioritized in marketing campaigns.

**Enhance loyalty initiatives**

Encourage repeat purchases to move customers into higher value segments.

---

# 🛠 Tech Stack

| Category             | Tools                  |
| -------------------- | ---------------------- |
| Data Cleaning        | Python (Pandas, NumPy) |
| Statistical Analysis | SciPy                  |
| Database             | MySQL                  |
| Visualization        | Power BI               |
| Version Control      | Git & GitHub           |

---

# 📁 Repository Structure

```
customer-shopping-behaviour-analysis
│
├── customer_shopping_behavior.csv
│   Raw dataset containing ~3,900 customer transactions
│
├── customer_shopping_behaviour_analysis.ipynb
│   Main analysis notebook
│   - Data cleaning
│   - Feature engineering
│   - Customer segmentation
│   - A/B testing simulation
│   - Pareto analysis
│   - Revenue impact modeling
│   - Visualization
│
├── create-customer-db.sql
│   SQL script used to create the MySQL database and tables
│
├── .env
│   Environment variables for secure database connection
│
└── README.md
    Project documentation
```

---

# ✨ Project Highlights

This project demonstrates several core analytics skills:

* Data cleaning and feature engineering
* SQL-based business analytics
* Customer segmentation
* Statistical hypothesis testing
* Revenue concentration analysis
* Business scenario modeling
* Dashboard storytelling

The analysis shows how **data can support strategic decision-making in retail and e-commerce environments.**

---