# Credit_Card_Expense_Analysis_Dashboard

## 📌 Project Objective

## 📊 Dashboards Overview

This project features two interactive **Power BI Dashboards**:

1. **Customer Dashboard**

   * Tracks customer demographics and behavior.
   * Includes visuals for:

     * Revenue by gender, state, marital status
     * Customer job vs revenue
     * Education level
     * Salary group, dependent count, and age group
     * Revenue trend over time

2. **Transaction Dashboard**

   * Focuses on transaction performance and cost metrics.
   * Includes:

     * Revenue by card category
     * Revenue by customer job and expenditure type
     * Annual fees, interest earned
     * Use of payment method (chip, swipe, online)
     * Acquisition cost by card tier
     * Quarterly trends in transaction volume and revenue

---

## 🧩 Data Sources

### 1. `customer.csv` / `Customer_c.csv`

Contains customer-related information including:

* Demographics (age, marital status, dependents, education, income)
* Card tier (Blue, Silver, Gold, Platinum)
* Employment details

### 2. `credit_card.csv` / `Client_c.csv`

Contains transactional details such as:

* Transaction amount and type
* Revenue and interest data
* Card usage patterns

---

## 🧪 SQL Logic

Custom SQL queries (`SQL Query (Financial).sql`) were used for:

* Aggregating customer and transaction data
* Calculating KPIs like revenue, interest, annual fees
* Joining multiple tables for enriched analysis

---

## 🛠 Tools & Technologies

* **Power BI** – Dashboard creation
* **SQL** – Data extraction and transformation
* **Excel** – Data cleaning and preprocessing
* **CSV Files** – Primary data input format

---

## 📈 Key Metrics Tracked

* 🧮 **Total Revenue**
* 💳 **Transaction Count & Amount**
* 📊 **Revenue by Category (Card, Job, Gender, Region, etc.)**
* 💰 **Customer Acquisition Cost**
* 📆 **Weekly & Quarterly Trends**
* 📎 **Interest Earned & Annual Fees**

---

## 📂 Folder Structure

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

## 👨‍💼 Author

**GOWTHAM GS PATIL**
Feel free to connect for any queries or collaborations!

---

## ✅ How to Use

1. Clone the repository:

   ```bash
   
   ```
2. Open the `.pbix` files in Power BI Desktop (coming soon).
3. Review the datasets and SQL logic in the respective folders.
4. Explore insights via dashboards in `/dashboards`.

