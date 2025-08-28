# Project Background

TransactIQ, a leading Nigerian fintech company, rolled out a major upgrade to its mobile and web applications on January 1, 2025, featuring a **redesigned user interface, new transaction flows, and backend infrastructure enhancements**. The upgrade was part of a broader strategy to improve user experience, reduce transaction failures, and strengthen customer trust.

Three months into the rollout, TransactIQ initiated a data-driven evaluation to **assess the performance of the new system and early feedback indicated a mix of improvements and challenges**, prompting leadership to commission a comprehensive analysis. The primary goal of this project was to find out users' friction points.

This project empowers TransactIQ’s teams to **track the actual impact of the app redesign**, identify opportunities for backend and frontend optimization, and quantify progress in key areas such as system reliability, and transaction throughput.

<br/>

### Key Analysis & Recommendation Areas

* **Post-Upgrade Transaction Funnel Breakdown**: Pinpoints where drop-offs spike across payment stages (wallet funding, or P2P transfers) in order to identify UX or backend bottlenecks introduced in the new app version.

* **Device Channel Usage vs Failure Rate**: Compares transaction reliability across devices (POS, mobile, USSD).

* **Customer Segmentation by Drop-Offs**

* **Revenue Recovered Through Retries Analysis**

<br/>

# Insights

### KPIs

**1.** Are Users Still Retrying Payments After the App Upgrade?

*Yes. The second window shows how many of those unique groups had multiple attempts.*

![Unique and Retries](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/bb8aa271599362a13328c8d61db55274cf8ee2a8/Resources/Unique%20%26%20Retries.png)

<br/>

<br/>

**2.** How Often Do Users Retry the Same Transaction?

*Nearly 1 in 4 transactions requires more than one attempt to complete.*

![Retry Rate](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/15e74efe1e552c887e4d8172c263c4d157e198b7/Resources/Retry%20Rate.png)

<br/>

<br/>

**3.** Are More Transactions Failing or Being Dropped?

*The 41% drop-off rate is a major friction or abandonment in transaction process as it indicates that nearly half of the users or systems initiating a transaction do not complete it. Likewise the 30% Failure Rate shows are likely technical or validation issues that prevent the transaction from succeeding.*

![Drop & Fail Rates](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/0ba55f68fdafc309bf1b12941809dc64ddf8570e/Resources/Drop%20%26%20Fail%20Rates.png)

<br/>

<br/>

**4.** How Many Customers Transact at High Value Customers?

*37 customers had over ₦15 million total transaction amount in 3 months.*

![High_Value_Customers](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/f6dc22919d0602996fa4e97f7374dbcc1592e11f/Resources/High_Value_Customers.png)


<br/>

<br/>

### Other Business Questions

**1.** What Is the Most Common Reason for Transaction Drop-Offs?

*The most frequent was Timeout, with 178 occurrences.*

![Top DropReason](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/f6dc22919d0602996fa4e97f7374dbcc1592e11f/Resources/High_Value_Customers.png)

















