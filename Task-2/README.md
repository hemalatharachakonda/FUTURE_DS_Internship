# Customer Churn Analysis – Task 2

##  Task Description
Analyze customer data to identify churn patterns, key retention drivers, and customer lifetime trends for a subscription‑based business.  
Deliverable: A retention analysis dashboard or report highlighting churn reasons, retention trends, and actionable recommendations to reduce customer loss.

##  Dataset
- **Source:** [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) (IBM sample dataset)
- **Rows:** 7,043 customers
- **Columns:** 21 features including customer demographics, account information, services subscribed, and churn status.

##  Tools Used
- Microsoft Excel
  - Pivot Tables
  - Charts & Slicers
  - Calculated Columns (Churn Flag, Tenure Groups)

##  Approach
1. **Data Cleaning**  
   - Checked for missing values in `TotalCharges` and replaced blanks with `0`.  
   - Converted `TotalCharges` to numeric format.  
   - Created a **Churn Flag** column (`1` for churned, `0` for retained) using `=IF(Churn="Yes",1,0)`.  
   - Created **Tenure Groups** to segment customers: `0-6 months`, `6-12 months`, `1-2 years`, `2+ years`.

2. **Exploratory Analysis via Pivot Tables**  
   - Churn rate by **Contract Type** (Month‑to‑month, One year, Two year).  
   - Churn rate by **Tenure Group**.  
   - Churn rate by **Payment Method**.  
   - Churn rate by **Internet Service** type.  
   - Average **Monthly Charges** for churned vs. retained customers.

3. **Dashboard Development**  
   - Combined key pivot charts into a single **Dashboard** sheet.  
   - Added **slicers** for `Contract`, `InternetService`, and `PaymentMethod` to enable interactive filtering.  
   - Displayed high‑level KPIs: Total Customers, Overall Churn Rate, Average Monthly Charges.

##  Key Insights
- **Contract Type:** Month‑to‑month contracts have the highest churn rate at **[XX]%**, compared to **[YY]%** for one‑year and **[ZZ]%** for two‑year contracts.
- **Tenure:** Customers in their first 6 months churn the most (**[AA]%**), indicating a critical onboarding period.
- **Payment Method:** Electronic check users churn at **[BB]%**, significantly higher than automatic payment methods (bank transfer: **[CC]%**, credit card: **[DD]%**).
- **Internet Service:** Fiber optic customers have a churn rate of **[EE]%** vs. DSL customers at **[FF]%**.
- **Tech Support:** Customers without tech support churn **[GG]%** more than those with tech support.
- **Monthly Charges:** Churned customers pay on average **[HH]** (currency) per month, while retained customers pay **[II]** – suggesting price sensitivity.

##  Recommendations
1. **Encourage Longer Contracts**  
   Offer incentives (e.g., first‑year discount, free installation) for month‑to‑month customers to switch to annual or two‑year plans.

2. **Enhance Onboarding for New Customers**  
   Implement a welcome program with proactive check‑ins, tutorials, and dedicated support during the first 6 months.

3. **Promote Tech Support**  
   Bundle tech support with popular internet packages or offer a free trial to demonstrate its value, especially for fiber optic users.

4. **Incentivize Automatic Payments**  
   Provide a small monthly discount for customers who switch from electronic check to bank transfer or credit card auto‑pay.

5. **Review Fiber Optic Pricing & Service Quality**  
   If fiber optic customers show high churn, assess competitive pricing and ensure reliable service; consider loyalty perks.


##  How to Use This Dashboard
- Open the Excel file `FUTURE_DS_02_Churn_Analysis.xlsx`.  
- Navigate to the **Dashboard** sheet.  
- Use the slicers at the top to filter by contract type, internet service, or payment method.  
- All charts and KPIs will update dynamically.

## ✅ Conclusion
This analysis provides a clear view of the key drivers of customer churn. By acting on the recommendations above, the business can reduce churn, improve customer retention, and increase lifetime value.
