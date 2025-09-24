📌 Project Overview
In this project, I analyzed the Shopify App Store to understand the factors that contribute to an app’s success. Using Power BI, I explored app data, reviews, and developer responsiveness to uncover insights that can guide both Shopify app developers and business owners when evaluating app performance.

📂 Dataset Description
The dataset consisted of four main tables:
*apps → Details of the apps on the Shopify marketplace
*apps_categories → Join table linking apps to categories
*categories → Categories of apps (each app may belong to multiple categories)
*reviews → User reviews (ratings, comments, and developer replies)

🛠️ Project Sections
Part 1: App Landscape
Objective: Understand the overall landscape of Shopify apps.
*Created a KPI Card showing the unique number of apps.
*Built a Line Chart showing the sum of review counts over time (lastmod date).
*Designed a Scatterplot plotting review count (X-axis) vs. average rating (Y-axis), with an interpretation box explaining the correlation.

Part 2: Reviews
Objective: Explore customer reviews and developer responsiveness.
*Created a calculated column helpful_reviews = rating * (1+helpful_count) to weigh reviews based on helpfulness.
*Built a Card to display the average of the helpful_reviews metric.
8Added a calculated column developer_answered = IF(NOT(ISBLANK([developer_reply])),1,0) to track whether developers responded to reviews.
8Designed a Scatterplot showing the relationship between average rating (Y-axis) and developer responsiveness (X-axis).

Part 3: App Reviews
Objective: Connect reviews with app and developer performance.
*Created a relationship between the Reviews table (app_id) and Apps table (id) to link user reviews to apps.
*Built a Bar Chart of developer (X-axis) vs. total ratings (Y-axis).
*Improved the visualization by replacing total ratings with average helpful_reviews, which accounts for review quality.
*Identified the most responsive developers using a bar chart filtered for apps with more than 500 reviews.

📂 Deliverables
Power BI Dashboard (.pbix) with three report pages:
App Landscape

Reviews
App Reviews
*Calculated DAX columns: helpful_reviews, developer_answered
*Visualizations showing app performance, review quality, and developer responsiveness

💡 Key Insights
Apps with higher review counts don’t always score higher in ratings, showing that popularity doesn’t guarantee quality.
Developers who respond to reviews tend to have higher average ratings, suggesting that engagement improves trust.
Some developers have thousands of reviews but lower helpful review scores, revealing gaps between volume and quality.
Filtering apps with 500+ reviews highlighted the most reliable and responsive developers in the Shopify ecosystem.

✨ This project demonstrates my ability to transform raw data into meaningful insights using Power BI—building KPIs, DAX measures, relationships, and interactive dashboards to tell a clear business story.
Do you also want me to add a placeholder link for your Power BI dashboard (so readers can interact with your visuals), or should this README only point to the dataset and deliverables?
