# SaaS-Revenue-Data-Exploration-and-Quality-Assessment

The data is quite **complete**, with no missing values, and it is also very **consistent** across the tables. The `customer_id` values **match correctly** between the `revenue` and `subscriptions` tables. 

However, I noticed something unusual in both the Monthly Recurring Revenue (MRR)and the monthly customer churn metrics.

For the **MRR**, it starts low, rises quickly, and stays fairly stable for several months. But toward the end of the year, it begins to **drop sharply**. As for **customer churn**, the early months look normal with a low churn rate, but by the final month, it **suddenly spikes dramatically**, to the point where **everyone churns**.

**Possible Causes:**

The sharp rise and fall in MRR may indicate simulated business cycles within the dataset, where customer activity is intentionally modeled to reflect periods of growth followed by decline. The sudden spike in churn at the end could also be the **result of artificially generated patterns** meant to help analysts practice detecting extreme churn scenarios rather than representing realistic customer behavior.

**Interpretation:**

These patterns suggest the dataset is **designed more for analytical training than for real-world forecasting**. While the data is structurally consistent, the extreme shifts should be treated as simulation artifacts rather than genuine market signals.
