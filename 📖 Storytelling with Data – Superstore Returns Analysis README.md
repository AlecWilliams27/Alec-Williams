📌 Project Overview

In this project, I investigated the high number of returned orders at the Superstore. My task was to prepare an analysis for the CEO to help them understand why customers are returning orders and how the business can reduce the overall volume of returns.
I used both data visualization and storytelling techniques to explore root causes, build a monitoring dashboard, and present my findings in a structured narrative.
Dataset used: Superstore.xls (Orders + Returns tables).

🛠️ Project Steps

1. What is Causing Returns?
I began by analyzing different views on return rates to uncover root causes.
Data Prep:
* LEFT JOINED the Returns table to the Orders table.
* Created a calculated field: IFNULL([Returned],0) where Yes = 1 and Null = 0.
8 Used this field to measure both return rates (average) and total returns (sum).

Visualizations Created:

* Scatterplot → Total sales vs. total returns (by product subcategory).
* Bar chart → Return rate by product category.
* Customer-level returns → Focused on customers with more than 1 order.
* Map → Return rate by geographic dimensions (state, city).
* Time-based analysis → Seasonal/temporal effects (month, week).
* Composite charts → Return rates by multiple factors (date + geography, product category + state, etc.).
* These visualizations allowed me to pinpoint patterns and anomalies in return behavior.

2. Building a Dashboard for Monitoring Returns

Next, I designed a dashboard in Tableau to monitor returns more effectively.
Mock-ups:
* Created at least 3 pen-and-paper sketches of potential dashboard designs.
* Selected my best option and aligned the layout with the key insights.

Dashboard Development:
* Built a dashboard template in Tableau using empty containers.
* Added visualizations (from Part 1) into the template.
* Finalized with clear titles, markers, and filters to make it user-friendly.
* The final dashboard allows executives to filter, explore, and interpret return data interactively.

3. Presenting My Analysis and Dashboard
The final step was to build a story arc and present my findings in a structured Tableau Story.

Story Draft:
* Summarized the scope of returns analysis.
* Evaluated how returns should be measured:
* Return rate → Highlights customer behavior.
* Total returns → Shows operational load.
* Total cost of returns → Quantifies financial impact.
* Outlined root causes of returns.
* Explained each component of the dashboard and how it should be interpreted.
* Demonstrated how filters can identify patterns in returns.

Story Presentation:
* Built a Tableau Story to guide executives through the findings.
* Proposed next steps, including:
* Implementing the dashboard as a monitoring tool.
* Taking corrective actions for high-return products/customers.
* Adjusting policies to reduce financial loss from returns.
* Delivered a 3–5 minute presentation (screen recording/PDF version).

📂 Deliverables
* Worksheets analyzing root causes of returns.
* Tableau Dashboard for monitoring returns.
* Tableau Story with captions and business narrative.
* 3–5 minute presentation of my findings.

💡 Key Insights
* Certain product subcategories generate high sales but also high returns, requiring closer review.
* Specific customers have abnormally high return rates and may need different handling strategies.
* Geographic and seasonal patterns show concentrations of return behavior.
* A centralized dashboard provides leadership with real-time monitoring and actionable insights.

✨ This project highlights my ability to not only analyze data but also craft a compelling narrative around it—turning numbers into insights that can directly influence executive decision-making.
