#  Credit Card Expense Analysis Dashboard

##  Project Objective

The primary goal of this project is to **analyze customer and transaction-level credit card data** to generate actionable insights using **Power BI Dashboards**. These insights help stakeholders understand customer behavior, revenue patterns, and cost breakdowns to improve business strategies.

---

##  Dashboard Overview

This project features two interactive **Power BI Dashboards**:

### 1.  Customer Dashboard

Focuses on customer demographics and revenue contribution.

**Key Visuals:**

* Revenue by gender, state, and marital status
* Job role vs revenue
* Education level distribution
* Salary group, number of dependents, and age group analysis
* Revenue trend over time

### 2.  Transaction Dashboard

Provides insights into transaction metrics and card usage trends.

**Key Visuals:**

* Revenue by card category (Silver, Gold, etc.)
* Expenditure by job role and type
* Interest earned, annual fees breakdown
* Payment method usage (chip, swipe, online)
* Customer acquisition cost by card tier
* Quarterly trends in transaction volume and revenue

---

##  Data Sources

### 1. `customer.csv` / `Customer_c.csv`

Contains customer demographic and employment data:

* Age, marital status, dependents
* Education, income level
* Card tier (Blue, Silver, Gold, Platinum)
* Occupation

### 2. `credit_card.csv` / `Client_c.csv`

Contains transaction-level data:

* Transaction amount, type, and method
* Revenue and interest generated
* Card usage behavior

---

##  SQL Logic

The `SQL Query (Financial).sql` script includes:

* Data aggregation and transformation
* Calculated KPIs (Revenue, Interest, Fees)
* Table joins for combined analysis
* Data filtering and grouping for Power BI

---

##  Tools & Technologies

* **Power BI** – Dashboard development & visualization
* **SQL** – Data querying, transformation, and aggregation
* **Microsoft Excel** – Data preprocessing and cleaning
* **CSV** – Raw data input format

---

##  Key Metrics Tracked

*  **Total Revenue Generated**
*  **Transaction Volume & Value**
*  **Revenue by Card Type, Gender, Job, Region**
*  **Customer Acquisition Cost (CAC)**
*  **Weekly, Monthly, and Quarterly Trends**
*  **Interest Earned & Annual Fees Collected**

---

##  Folder Structure

```bash
Credit_Card_Dashboard_Project/
│
├── data/
│   ├── customer.csv
│   ├── credit_card.csv
│   └── Client_c.csv
│
├── dashboards/
│   ├── Credit_Card_Customer_Dashboard.pdf
│   └── Credit_Card_Transaction_Dashboard.pdf
│
├── sql/
│   └── SQL Query (Financial).sql
│
└── README.md
```

---

##  How to Use

1. **Clone the repository:**

   ```bash
   git clone https://github.com/gowthamgspatil/Credit_Card_Expense_Analysis_Dashboard.git
   ```

2. **Explore the SQL script:**

   * Open the `sql/SQL Query (Financial).sql` file in any SQL editor.
   * Understand how data is transformed and KPIs are derived.

3. **Review the Dashboards:**

   * View the dashboard PDFs in the `/dashboards` folder.
   * (.pbix files will be available soon for full interactivity in Power BI Desktop.)

4. **Inspect the data:**

   * Go to the `data/` folder and explore the `.csv` files used in this project.

---

# Author

**Gowtham GS Patil**

*  [LinkedIn](https://www.linkedin.com/in/gowthamgshivamuthy)
*  [Email](mailto:gowthamgshivamurthy@gmail.com)

Feel free to reach out for collaboration, questions, or feedback!

---

## 📣 Acknowledgements

* This project is part of a personal data analytics portfolio.
* Inspired by real-world financial datasets to practice **data modeling**, **KPI analysis**, and **Power BI reporting**.
