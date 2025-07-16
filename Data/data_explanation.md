Here is a **summary explanation** of the four Excel (CSV) files you uploaded:

---

### 🔹 1. **Client\_c.csv** (185 records, 18 columns)

This file contains summarized **credit card transaction and profile information** for 185 clients.

| Column                                               | Description                                             |
| ---------------------------------------------------- | ------------------------------------------------------- |
| `Client_Num`                                         | Unique client identifier                                |
| `Card_Category`                                      | Type of credit card (e.g., Blue)                        |
| `Annual_Fees`                                        | Yearly fee charged for the card                         |
| `Activation_30_Days`                                 | Whether card was activated in 30 days (1 = Yes, 0 = No) |
| `Customer_Acq_Cost`                                  | Cost to acquire the customer                            |
| `Week_Start_Date`, `Week_Num`, `Qtr`, `current_year` | Temporal details about when the data was captured       |
| `Credit_Limit`                                       | Maximum credit limit allowed                            |
| `Total_Revolving_Bal`                                | Balance carried month-to-month                          |
| `Total_Trans_Amt`                                    | Total amount spent on transactions                      |
| `Total_Trans_Ct`                                     | Count of transactions                                   |
| `Avg_Utilization_Ratio`                              | Ratio of credit used to limit                           |
| `Use Chip`, `Exp Type`                               | How the card is used and spending category              |
| `Interest_Earned`                                    | Interest earned from the account                        |
| `Delinquent_Acc`                                     | Number of times account was delinquent                  |

---

### 🔹 2. **credit\_card.csv** (10,108 records, 18 columns)

This is a **detailed version of Client\_c.csv** — same structure, but with full data from all customers.

💡 **Difference from Client\_c.csv**:

* Larger dataset (full population vs. sample)
* One additional column: `Total_Trans_Vol` (number of swipes/transactions)

---

### 🔹 3. **customer.csv** (10,108 records, 15 columns)

This dataset contains **demographic and personal info** of customers.

| Column                                      | Description                                        |
| ------------------------------------------- | -------------------------------------------------- |
| `Client_Num`                                | Unique client ID (links to credit card dataset)    |
| `Customer_Age`, `Gender`, `Dependent_Count` | Age, gender, and number of dependents              |
| `Education_Level`, `Marital_Status`         | Educational qualification and marital status       |
| `state_cd`, `Zipcode`                       | Geographic data                                    |
| `Car_Owner`, `House_Owner`                  | Asset ownership indicators                         |
| `Personal_loan`                             | Whether the customer has a personal loan           |
| `contact`                                   | Preferred contact method (e.g., cellular, unknown) |
| `Customer_Job`                              | Job category (e.g., Businessman, Blue-collar)      |
| `Income`                                    | Annual income                                      |
| `Cust_Satisfaction_Score`                   | Customer satisfaction score (1–5 scale)            |

---

### 🔹 4. **Customer\_c.csv** (185 records, 15 columns)

This is a **subset/sample** of `customer.csv` – contains only 185 customer records, likely matching the sample in `Client_c.csv`.

---

### ✅ Summary of Usage:

You can **merge** `Client_c.csv` with `Customer_c.csv` (or the full files) on `Client_Num` to create a **complete customer profile**, useful for:

* Credit risk analysis
* Customer segmentation
* Churn prediction
* Marketing targeting

Let me know if you'd like a merged version or visual summary!
