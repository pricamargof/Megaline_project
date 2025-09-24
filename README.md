Which Plan is Better?

This project analyzes customer data from the telecommunications company Megaline, which offers two prepaid plans: Surf and Ultimate. The commercial department wants to identify which plan generates higher revenue in order to adjust the advertising budget.

The dataset contains information on 500 customers: who they are, where they live, which plan they use, and the number of calls and messages they made in 2018. The goal is to analyze customer behavior, determine which plan yields more revenue, and test whether the average revenue of users in the NY-NJ area differs from that of users in other regions.

General Process

Data Preparation: Corrected data types (dates converted from object to datetime), removed zero-value calls and sessions, rounded call minutes up, and created a new column (gb_used) to calculate internet usage in gigabytes.

Data Aggregation: Built a consolidated DataFrame (df_final) grouped by user and month, containing calls, minutes, messages, data usage, plan type, region, and monthly revenue.

Exploratory Analysis: Visualized user behavior with plots showing average call duration, average number of messages per month, and average internet usage per month. User behavior between Surf and Ultimate plans appeared broadly similar.

Revenue Analysis:

Average monthly revenue: Ultimate = $72, Surf = $60.

Additional revenue from exceeding plan limits came mainly from Surf users.

The majority of revenue originated from the NY-NJ-PA MSA region.

Statistical Testing: Hypothesis tests confirmed that differences in average revenue between plans and between regions are statistically significant.

Final Conclusion

The Ultimate plan generates higher average revenue and should be prioritized in advertising campaigns. Additionally, marketing efforts should focus on the NY-NJ-PA MSA region, which contributes the largest share of total revenue.
