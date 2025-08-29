# Project Background

TransactIQ, a leading Nigerian fintech company, rolled out a major upgrade to its mobile and web applications on January 1, 2025, featuring a **redesigned user interface, new transaction flows, and backend infrastructure enhancements**. The upgrade was part of a broader strategy to improve user experience, reduce transaction failures, and strengthen customer trust.

Three months into the rollout, TransactIQ initiated a data-driven evaluation to **assess the performance of the new system and early feedback indicated challenges**, prompting leadership to commission a comprehensive analysis. The primary goal of this project was to find out users' friction points.

This project empowers TransactIQ’s teams to **track the actual impact of the app redesign**, identify opportunities for backend and frontend optimization, and quantify progress in key areas such as system reliability, and transaction throughput.

<br/>

### Key Analysis & Recommendation Areas

* **Post-Upgrade Transaction Funnel Breakdown**: Pinpoints where drop-offs spike across payment stages (wallet funding, or P2P transfers) in order to identify UX or backend bottlenecks introduced in the new app version.

* **Device Channel Usage vs Failure Rate**: Compares transaction reliability across devices (POS, mobile, USSD).

* **Customer Segmentation by Drop-Offs**

* **Revenue Recovered Through Retries Analysis**

<br/>

<br/>

# Executive Summary

Over a 3-month transactional review period, performance indicators revealed **persistent revenue loss**, particularly relating to transaction **drop-offs and failed recoveries**.

The most critical insight comes from the retry recovery analysis. Across all dropped transactions, **the platform failed to recover even a single payment through retries**. **Not one customer who experienced a failed attempt went on to successfully complete that same transaction through a subsequent attempt**. This shows that once a transaction fails, it’s gone permanently. Whether the failure was due to technical errors, insufficient funds, or customer abandonment, there is no systematic re-engagement: **no push to retry, no saved progress, no follow-up**.

In essence, **TransactIQ's platform has no functional retry funnel** as it shows thousands of potential revenue opportunities are lost without recapture. Even a modest recovery rate of 10–20% on retries could have reversed this trend significantly. But currently, the infrastructure is allowing users to fail once and never return.

These findings point to a need for comprehensive workflow redesigns: **from preemptive drop-off prevention to post-failure re-engagement mechanisms (such as retry prompts, saved transaction states, and smarter customer nudges)**. Without this, the platform will continue to suffer silent but substantial revenue leakage and declining customer trust.

<br/>

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

![High_Value_Customers](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/b150efa20aec0f610374f3550bfb78815d4f8b5f/Resources/high_value_customers.png)


<br/>

<br/>

### Other Business Questions

**1.** What Is the Most Common Reason for Transaction Drop-Offs?

*The most frequent was Timeout, with 178 occurrences.*

![Top DropReason](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/19037d6108c6ede8078e2ba979887823cce7deeb/Resources/top%20dropreasoncode.png)

<br/>

<br/>

**2.** At Which Stages Do Most Customers Drop Off During the Transaction Funnel?

*The three most common drop-off points in the transaction process are Confirmation Stage, Amount Entry Stage, and OTP Stage*

![Fail Points](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/16b456e9a1febc37684c9eaf6812686a31b40481/Resources/fail%20points.png)

<br/>

<br/>

**3.** Are users more likely to drop off when paying bills, sending money, or topping up airtime? 

*Wallet Funding is the transaction type with the highest number of drop-offs, totalling 5,590 instances.*

![Likely to drop off](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/4686a0a10bf318f2006665bdf5436c5ddff972b8/Resources/likeliness.png)

<br/>

<br/>

**4.** Which devices have higher failure or drop-off rates?

*The Web platform has the highest number of transaction failures and drop-offs, followed closely by POS terminals and Tablets.

![Device Drop Off Rate](https://github.com/Blessing336/Transaction_Drop-Off_Analysis_for_TransactIQ_-SQL_Project-/blob/ffe13cf642474127f71c0cf00ed3e0354c4bdcba/Resources/device%20drop%20dff%20rate.png)

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

<br/>

<br/>

# Recommendations

1. **Implement Pre-Transaction Affordability Checks**

*4,312 drop-offs occurred due to customers attempting transactions beyond their available balance.*

These are avoidable failures. Customers should never have to reach the point of transaction failure if balance checks are done early and clearly communicated.

**Solution: Introduce real-time balance validation before a transaction progresses past the review screen.**

<br/>

<br/>

2. **Design and Deploy a Smart Retry Funnel**

*Zero transactions were recovered through retries — representing complete revenue loss once a transaction fails.*

Customers may be willing to complete a transaction if prompted or reminded, especially if the cause was a temporary issue (low balance, network issue).

**Solution:**
* Save failed transaction details temporarily, allowing users to retry within a set time window (e.g., 30 mins).

* Trigger automated reminders via SMS, email, or push notification to prompt retry.

* Use smart retry logic ie. If the failure was due to low balance, prompt when balance is restored.

<br/>

<br/>

3. **Set Up Weekly Drop-Off Analytics & Recovery Dashboards**

A real-time monitoring system helps the business stay proactive, not reactive.

**Solution:**

* Build a Power BI dashboard showing: Drop-off trends over time, Drop-offs by cause, Retry attempts vs successes, Trigger alerts when drop-offs spike unexpectedly.



<br/>

<br/>





Go to my GitHub *[Home Page](https://github.com/Blessing336)*






