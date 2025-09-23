📌 Project Overview

I was hired as a junior analyst at an e-commerce company to transform raw transaction logs into actionable business metrics. Each row in the dataset represented a user activity (product views, cart opens, or purchases) on the company’s website. My goal was to explore the dataset, clean and organize the data, and deliver insights that the executive team could use to evaluate conversion performance and customer retention.

Check out the dashboard here [https://docs.google.com/spreadsheets/d/e/2PACX-1vTnOYgEHvw3YJam_N-YmHF55ES_t6viVM_KdXKAA3-pQk1nZTRIH2CwfFdrmGxJd65MDa61hDqLiEBK/pubhtml]

📂 Dataset Description

The dataset contained event-level activity with the following columns:
* user_id → Unique customer ID
* event_type → Type of activity (view, cart, purchase)
* category_code → Product category being viewed or purchased
* brand → Company that makes the product
* price → Price of the product (USD)
* event_date → Date of activity (YYYY-MM-DD)

🛠️ Project Steps
Part 1: Conversion Funnel
* The first task was to evaluate how well the site converts product page views into purchases.
* I built a pivot table in a new sheet called conversion_funnel.
* I counted unique users at each stage (views → carts → purchases).

I created two calculated columns:
* Total Conversion Rate (views → purchase).
* Step-to-Step Conversion Rate (e.g., view → cart, cart → purchase).
* This provided visibility into drop-offs at each step of the funnel.

Part 2: Preparing Data for Cohort Analysis
* To track customer acquisition and retention, I prepared data for a cohort analysis.
Filtered Purchases
* Isolated purchase events into a new sheet called purchase_activity.
* Ensured only purchase rows were included (4,845 rows).
* Calculated First Purchases
* Created a pivot table in a sheet called first_purchase.
* Found the minimum purchase date for each user.
* Used VLOOKUP() to pull these dates into the purchase_activity sheet.

Created Cohort Columns:
* event_month → =TEXT(event_date,"YYYY-MM")
* first_purchase_month → =TEXT(first_purchase_date,"YYYY-MM")
* cohort_age → =DATEDIF(first_purchase_date,event_date,"m")
* These columns allowed me to group purchases by acquisition month and track activity over time.

Part 3: Retention Rates
* I then aggregated purchase activity into cohorts and calculated monthly retention.
Built a pivot table in cohort_analysis where:
* Rows = Cohorts (based on first purchase month).
* Columns = Cohort age (0 to 4 months).
* Values = Unique users.
In a new sheet called retention_rates:
*I calculated retention rates by dividing active users in later months by the starting size of the cohort.
* This showed how well the company retains customers month over month.

Part 4: Organizing & Documenting the Spreadsheet
* To make the project polished and professional for executives:
* Wrote an Executive Summary with results and analysis notes.
* Documented data assumptions (e.g., reviews reflect actual stays, retention measured by repeat purchases).
Reordered sheets for clarity:

❇️ Table of Contents
* Executive Summary
* Analytical results (conversion funnel, retention rates, cohort analysis)
Supporting calculations (purchase activity, first purchase)
* Raw data (raw_user_activity)
Applied formatting: borders, bold headers, frozen rows, formatted dates/numbers, and clear labels.

📊 Key Deliverables
* Conversion Funnel → User journey from view → cart → purchase.
* Purchase Activity → Filtered dataset of purchases only.
* First Purchase Sheet → Cohort assignments by first purchase month.
* Cohort Analysis → Pivot table showing user retention by cohort.
* Retention Rates Sheet → Calculated retention percentages month-over-month.
* Executive Summary → High-level results and business implications.

💡 Business Insights
The funnel highlighted where the company loses the most customers during checkout.
Cohort analysis showed retention varies by acquisition month, helping the company understand seasonal patterns and long-term customer value.
These insights can guide improvements to the conversion flow and help design strategies for customer retention.

✨ This project demonstrates my ability to turn raw event logs into meaningful business metrics using advanced spreadsheet techniques such as pivot tables, VLOOKUP, TEXT(), and DATEDIF().
