###  **0. Create the Database**

```sql
CREATE DATABASE ccdb;
```

Creates a new database called **`ccdb`** (short for *Credit Card Database*).

---

###  **1. Create Table: `cc_detail`** (Credit Card Transaction Data)

```sql
CREATE TABLE cc_detail (
    Client_Num INT,
    Card_Category VARCHAR(20),
    Annual_Fees INT,
    Activation_30_Days INT,
    Customer_Acq_Cost INT,
    Week_Start_Date DATE,
    Week_Num VARCHAR(20),
    Qtr VARCHAR(10),
    current_year INT,
    Credit_Limit DECIMAL(10,2),
    Total_Revolving_Bal INT,
    Total_Trans_Amt INT,
    Total_Trans_Ct INT,
    Avg_Utilization_Ratio DECIMAL(10,3),
    Use_Chip VARCHAR(10),
    Exp_Type VARCHAR(50),
    Interest_Earned DECIMAL(10,3),
    Delinquent_Acc VARCHAR(5)
);
```

 **Purpose**: Stores transaction and financial metrics
 **Key Columns**:

* `Client_Num`: Unique customer ID
* `Annual_Fees`, `Credit_Limit`, `Total_Trans_Amt`, etc.
* `Use_Chip`, `Exp_Type`: How and where card was used
* `Interest_Earned`, `Delinquent_Acc`: Credit performance

---

###  **2. Create Table: `cust_detail`** (Customer Demographics)

```sql
CREATE TABLE cust_detail (
    Client_Num INT,
    Customer_Age INT,
    Gender VARCHAR(5),
    Dependent_Count INT,
    Education_Level VARCHAR(50),
    Marital_Status VARCHAR(20),
    State_cd VARCHAR(50),
    Zipcode VARCHAR(20),
    Car_Owner VARCHAR(5),
    House_Owner VARCHAR(5),
    Personal_Loan VARCHAR(5),
    Contact VARCHAR(50),
    Customer_Job VARCHAR(50),
    Income INT,
    Cust_Satisfaction_Score INT
);
```

 **Purpose**: Holds personal and demographic information
 **Key Columns**:

* `Customer_Age`, `Gender`, `Education_Level`
* `Income`, `Customer_Job`, `Cust_Satisfaction_Score`

---

###  **3. Import CSV Data (PostgreSQL `COPY`)**

#### Load data into `cc_detail`:

```sql
COPY cc_detail
FROM 'D:\credit_card.csv'
DELIMITER ','
CSV HEADER;
```

#### Load data into `cust_detail`:

```sql
COPY cust_detail
FROM 'D:\customer.csv'
DELIMITER ','
CSV HEADER;
```

 If you get date format errors like:

```
ERROR: date/time field value out of range: "0"
```

You can fix it by running:

```sql
SET datestyle TO 'ISO, DMY';
```

Or by fixing the CSV values to standard `YYYY-MM-DD`.

---

###  **4. Append Additional Data**

Assuming you have Week-53 data in new CSVs:

#### Append to `cc_detail`:

```sql
COPY cc_detail
FROM 'D:\cc_add.csv'
DELIMITER ','
CSV HEADER;
```

#### Append to `cust_detail`:

```sql
COPY cust_detail
FROM 'D:\cust_add.csv'
DELIMITER ','
CSV HEADER;
```

---

###  **Overall Purpose**

This script:

1. **Creates schema** for customer and transaction data
2. **Loads data** from multiple CSV files
3. **Supports PostgreSQL** and offers tips for common errors
4. Helps build a **data warehouse** or Power BI backend for credit card customer analytics


