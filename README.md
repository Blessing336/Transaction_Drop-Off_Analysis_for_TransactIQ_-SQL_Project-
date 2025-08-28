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

![Unique and Retries](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/61a0d38f69e0fdfb2a6c9ea9ec98569a3fe23787/Resources/unique%20%26%20retries.png)

<br/>

<br/>

**2.** How Often Do Users Retry the Same Transaction?

*Nearly 1 in 4 transactions requires more than one attempt to complete.*

![Retry Rate](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/bdb232267409fcea845363a26cb66f60597f865c/Resources/retry%20rate.png)

<br/>

<br/>

**3.** Are More Transactions Failing or Being Dropped?

*The 41% drop-off rate is a major friction or abandonment in transaction process as it indicates that nearly half of the users or systems initiating a transaction do not complete it. Likewise the 30% Failure Rate shows are likely technical or validation issues that prevent the transaction from succeeding.*

![Drop & Fail Rates](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/b6ec0b707b96fb05e5a2445f5da7e9bee969feb6/Resources/drop%20%26%20fail%20rates.png)

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

![Top DropReason](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/d3d47a173a311b47de6ee85f88794f260f19d53b/Resources/Top%20DropReasonCode.png)

<br/>

<br/>

**2.** At Which Stages Do Most Customers Drop Off During the Transaction Funnel?

*The three most common fail points in the transaction process are Confirmation Stage, Amount Entry Stage, and OTP Stage*

![Fail Points](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/3ad12f76246060dd666267f44129a74c80af423a/Resources/Fail%20Points.png)

<br/>

<br/>

**3.** Are users more likely to drop off when paying bills, sending money, or topping up airtime? 

*Wallet Funding is the transaction type with the highest number of drop-offs, totalling 5,590 instances.*

![Likely to drop off](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/d81b009460440d0247c2ea9aaf224bcc5678b8ff/Resources/Likeliness.png)

<br/>

<br/>

**4.** Which devices have higher failure or drop-off rates?

*The Web platform has the highest number of transaction failures and drop-offs, followed closely by POS terminals and Tablets.

![Device Drop Off Rate](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/5b78d47ed3cf078a38c58700e899df24ed0811bb/Resources/Device%20Drop%20Off%20Rate.png)

<br/>

<br/>

**5.** What Was the Total Value of Dropped Transactions in the Last Three Months?

*Compared to January, there is a steady decrease in the value of dropped transactions over the three months, with March seeing the second to the lowest drop-off value exceeding ₦240 million.*

![Monthly Drop Off Rate](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/ddf027dbeb8985791a73ffa55bf793caebb1b9b6/Resources/Drop%20off%20Month.png)

<br/>

<br/>

**6.** How Many Drop-Offs Were Caused by Insufficient Balance?

*4,312 attempted payments failed, not due to system errors or device issues, but because customers didn’t have enough money at the time of the transaction.*

![Insufficient Balance](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/c7e0c0b2c7748914394c1112337b73f4445a2348/Resources/insufficient%20balance.png)

<br/>

<br/>

**7.** How Much Revenue Was Recovered Through Retries?

* Every failed transaction is a permanent loss because zero transactions were successfully completed after failed attempts. Customers who experienced a transaction drop-off never returned to retry or complete their purchases.

![Retries Recovered](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/d028696cf52a05f8f29148f297f1a16ebe453f86/Resources/Retries_Recovered.png)














