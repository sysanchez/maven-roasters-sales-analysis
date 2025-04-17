# Maven Roasters Sales Analysis (Jan 2023 - June 2023)

## Key Sections

  - [Background and Overview](#background-and-overview)
  - [Data Structure Overview](#data-structure-overview)
  - [Executive Summary](#executive-summary)
  - [Deep-dive Insights](#deep-dive-insights)
  - [Recommendations](#recommendations)
  - [Limitations](limitations)
    
## Background and Overview: 
Maven Roasters is a coffee shop chain with three locations in New York City: Astoria, Hell’s Kitchen, and Lower Manhattan.

This analysis aims to identify revenue trends, bestselling products, peak transaction times, and key revenue drivers across Maven Roasters’ three NYC locations. The goal is to provide insights that help the business owner better understand customer purchasing behavior, recognize trends and opportunities, and optimize operations to maximize sales and profitability.

Insights and recommendations focus on three key areas:
- **Sales Trends Over Time** – Understanding revenue patterns and growth opportunities.
- **Sales Volume by Day and Time** – Identifying high-traffic periods to optimize operations.
- **Product Performance and Revenue Drivers** – Highlighting top-selling items and areas for improvement.
  
## Data Structure Overview

The dataset provided in a single table represents sales data, where every single record represents a transaction. There are 149, 456 transactions in the data set and each row represents a single transaction, detailing the date, time, location, and product quantity as well as the product-level details such as the product id, category and type, product detail, quantity purchased, and sales price.

Here is the list of all the columns from the given table of data:
Transaction Details: transaction_id, transaction_date, transaction_time, transaction_qty
Store Information: store_id, store_location
Product Information: product_id, product_category, product_type, product_detail, unit_price

The dataset covers transactions from January 2023 to June 2023.

The dataset is available [here](https://github.com/sysanchez/maven-roasters-sales-analysis/blob/0ec670a59f92e92300df94663f7ac205d9daab4a/Coffee%20Shop%20Sales%20Dataset%20(Raw).xlsx).

View the data exploration and analysis report [here](https://github.com/sysanchez/maven-roasters-sales-analysis/blob/02f1e453dd8e887ea14cc59caee5a7f622a9423a/Data%20Cleaning%2C%20Exploration%20%26%20Analysis.pdf).

## Executive Summary

From January to June, sales across the three Maven Roasters locations followed an upward trend, peaking in June with each store generating more than $50,000 in revenue — double the amount generated in January. February saw a slight decline in all stores, possibly due to lower post-holiday consumer spending or seasonal fluctuations in customer traffic with declines amounting to $2,209 in Astoria, $2,101 in Hell's Kitchen, and $1,223 in Lower Manhattan.

The busiest days vary by store, but weekdays generally see the highest number of transactions. In Astoria, Thursday has the most transactions (7,427), followed closely by Monday (7,403) and Wednesday (7,370). Hell's Kitchen sees the highest transaction volumes on Friday (7,489) and Tuesday (7,572), while in Lower Manhattan, Monday is the busiest day (7,136).

Coffee is the best-selling category across all stores, with 20,025 transactions in Astoria, 20,187 in Hell’s Kitchen, and 18,204 in Lower Manhattan. Barista Espresso leads in both transactions and revenue in Hell’s Kitchen (6,153 transactions, $32,420 revenue) and Lower Manhattan (5,320 transactions, $31,051 revenue). In contrast, Astoria’s top-selling item is Brewed Chai Tea, generating 6,293 transactions and $27,428 in revenue. Syrups (regular and sugar-free) had the lowest sales across all stores, with total transactions ranging from around 400 to 2,100 and revenue between $450 and $2,600, indicating they are primarily add-ons rather than standalone purchases.

Below is a screenshot of the dashboard in Excel. The entire interactive dashboard can be downloaded [here](https://github.com/sysanchez/maven-roasters-sales-analysis/blob/0ec670a59f92e92300df94663f7ac205d9daab4a/Coffee%20Shop%20Sales%20Dashboard.xlsx).

![Lower Manhattan Sales Dashboard](https://github.com/sysanchez/maven-roasters-sales-analysis/blob/0ec670a59f92e92300df94663f7ac205d9daab4a/Maven%20Roasters%20Sales%20Dashboard%20SS.png)

## Deep-dive Insights

### Astoria

**Sales Trends Over Time**

![Total Revenue by Month in Astoria](https://github.com/user-attachments/assets/8150ff8b-3156-4331-8f94-bdbc2887a986)

Total revenue showed steady growth, increasing from $27,314 in January to $55,083 in June, reflecting a 101% increase over six months. There was a slight dip in February, likely due to post-holiday spending slowdowns, but things picked up again in March and continued to grow. June marked the highest revenue, likely driven by increased customer demand or seasonal trends.

**Busiest Days of the Week & Busiest Hours of the Day**

![Transactions by Day of Week in Astoria](https://github.com/user-attachments/assets/e86b373f-1d04-410e-97a3-5f4479a23f24)  

Transactions vary throughout the week, with the highest activity on Thursday (7,427transactions) and the lowest on Saturday (6,942 transactions). Monday, Wednesday, and Friday see strong sales with over 7,000 transactions, while weekend transactions are lower, likely due to lower foot traffic on Saturdays and Sundays.

![Transactions by Hour of Day in Astoria](https://github.com/user-attachments/assets/f84a392e-1861-4d33-8f58-1f859bc7e187)

The busiest time of the day is between 9 AM and 10 AM, with transactions exceeding 5,000. After 11 AM, sales drop to around 3,000 per hour and remain steady throughout the afternoon. This trend suggests high demand for morning coffee, while afternoon sales remain consistent but lower.

**Product Performance & Revenue Drivers**

![Transactions by Product Category in Astoria](https://github.com/user-attachments/assets/87800a46-f238-41a6-b6a4-966046becc9f)  

Coffee is the best-selling product category, with 20,025 transactions, followed closely by tea at 16,260. Bakery items also see strong sales, with more than 7,289 transactions, while categories like packaged chocolate and branded merchandise have significantly lower sales, with fewer than 400 transactions each. This suggests that customers primarily visit for beverages, with food as a secondary purchase, while packaged retail items see limited demand.

![Top 15 Products in Astoria](https://github.com/user-attachments/assets/a31578f7-775f-41dd-823a-19894309a63c)

Brewed Chai Tea leads in transactions with over 6,200 sales, generating nearly $27,500 in revenue, while Barista Espresso, despite having fewer transactions (4,930), brings in a similar amount of revenue. Regular and sugar-free syrups have the lowest sales, with fewer than 1,200 combined transactions and under $2,000 in revenue, reinforcing their role as add-ons rather than primary purchases. Overall, brewed beverages dominate both sales and revenue, highlighting customer preference for handcrafted drinks.

### Hell’s Kitchen

**Sales Trends Over Time**

![Total Revenue by Month in Hell's Kitchen](https://github.com/user-attachments/assets/21b9554d-6322-48c2-996c-c6d70abd2875)

Total revenue steadily increased over six months, with a small dip of $2,101 in February before reaching $56,957 in June. The most significant growth occurred between April and May, with an increase of over $12,000, possibly driven by seasonal demand, marketing efforts, or higher customer traffic.

**Busiest Days of the Week & Busiest Hours of the Day**

![Transactions by Day of Week in Hell's Kitchen](https://github.com/user-attachments/assets/0e1df456-62ab-4cad-b43a-a77af897f514)

Tuesday and Friday saw the highest number of transactions, with 7,472 and 7,489, respectively, indicating strong midweek and end-of-week sales. Saturday had the lowest transaction count at 6,846, suggesting a slight dip in weekend activity. Overall, transactions remained fairly consistent throughout the week.

![Transactions by Hour of Day in Hell's Kitchen](https://github.com/user-attachments/assets/4a9243db-e404-47de-8517-0b608329dc7f)

Transactions peak in the morning, with the highest volume at 9 AM (6,909 transactions) and 10 AM (6,767 transactions), highlighting strong demand during early hours. Activity gradually declines throughout the day, with the lowest number of transactions recorded at 8 PM (528). This suggests that most customers visit earlier in the day, likely for their morning coffee or breakfast.

**Product Performance & Revenue Drivers**

![Transactions by Product Category in Hell's Kitchen](https://github.com/user-attachments/assets/fa74eff2-0499-4d40-a9ea-0d7fe11a784c)

Coffee leads in sales with 20,187 transactions, followed by bakery items with 7,617 and drinking chocolate with 3,763, while other categories see lower demand. Branded products (119 transactions) and packaged chocolate (197 transactions) have the fewest sales, suggesting they appeal to a smaller, niche customer base.

![Top 15 Products in Hell's Kitchen](https://github.com/user-attachments/assets/4853701e-5767-4a52-99f4-3c4ae82931a0)

Barista Espresso leads in revenue, generating $32,420 from 6,153 transactions, showing strong customer preference for premium coffee options. Brewed Chai Tea follows closely with $25,645 in revenue, despite slightly fewer transactions at 5,824, indicating higher pricing or larger order sizes. In contrast, sugar-free syrup has the lowest revenue at just $718 from 602 transactions, suggesting limited demand for specialty add-ons.

### Lower Manhattan

**Sales Trends Over Time**

![Total Revenue by Month in Lower Manhattan](https://github.com/user-attachments/assets/25ae118f-6c71-4688-81b2-e29b860f4bd2)

Revenue showed a strong upward trend, increasing from $26,543 in January to $54,446 in June, more than doubling over six months. The most significant jump occurred between April and May, with a $12,541 increase, suggesting higher customer demand or successful business strategies. This consistent growth highlighted strong performance momentum and potential for further expansion.

**Busiest Days of the Week & Busiest Hours of the Day**

![Transactions by Day of Week in Lower Manhattan](https://github.com/user-attachments/assets/c399897e-57de-4660-a1e6-a382e1b0aee7)

Monday is the busiest day of the week, with 7,136 transactions, slightly ahead of Thursday at 6,920. Weekday transactions remain fairly consistent, while weekends see a small dip, with Saturday (6,722) and Sunday (6,679) having the lowest activity. This suggests that customer traffic is higher during the workweek, potentially due to routine coffee runs or office-related purchases.

![Transactions by Hour of Day in Lower Manhattan](https://github.com/user-attachments/assets/fcdf8f02-e747-4113-ae97-2293adf4787e)

Morning hours are the busiest, with transactions peaking around 10 AM at over 6,000. The early rush begins at 6 AM and remains strong through 9 AM, likely driven by commuters and morning routines. After 11 AM, transactions drop significantly and gradually decline through the afternoon, with minimal activity after 6 PM.

**Product Performance & Revenue Drivers**

![Transactions by Product Category in Lower Manhattan](https://github.com/user-attachments/assets/58cf0f18-b5b4-4e38-b4a4-5db24667b00b)

Coffee is the top-selling category with 18,204 purchases, surpassing tea at 13,912. Bakery items follow with 7,890 transactions, making them the top non-beverage choice. Meanwhile, niche products like packaged chocolate (180) and branded items (349) have the lowest sales, indicating a smaller customer base.

![Top 15 Products in Lower Manhattan](https://github.com/user-attachments/assets/68023999-ba1f-4d6e-95ef-66f2841bcd6f)

Barista Espresso leads in both transactions (5,320) and revenue ($31,051), making it the top-performing product. Gourmet brewed coffee and brewed chai tea also drive strong sales, generating over $23,000 each. Meanwhile, sugar-free syrup has the lowest figures, with only 830 transactions and $1,153 in revenue, indicating lower demand compared to core beverage offerings.

## Recommendations

Based on the key insights identified, the following recommendations are proposed.

***Boost total revenue by addressing the February dip & maximizing growth from April to June (All Stores)***

- To minimize the February slowdown across all stores, launch a mid-winter promotion such as "Warm Up February" discounts on seasonal drinks and pastries, introduce a limited-time winter menu featuring specialty hot chocolates and comfort pastries, and offer a loyalty incentive like bonus points for February purchases to encourage repeat visits.
- To capitalize on Spring Growth from April to June across all stores, introduce a Spring/Summer drink lineup featuring iced coffee specials and refreshing tea blends and promote bundle deals such as the “Morning Boost” combo of coffee and pastry at a discount.

***Maximize Weekday Sales and Boost Weekend Traffic (All Stores)***

- To make the most of peak weekday traffic, Maven Roasters could offer targeted promotions or loyalty incentives on these high-traffic days to boost sales further.
- To boost weekend sales, run weekend promotions (e.g., "Buy 1, Get 1 Free" on slow-moving items like packaged chocolate), offer exclusive weekend-only drinks or bundles to attract customers or partner with local businesses for weekend collaborations (e.g., pastry pairings from a local bakery).

***Optimize Store Hours and Promotions for Peak and Slow Periods (Store-specific adjustments)***

- Astoria: Focus on improving efficiency during the busy 9-10 AM window with faster checkout and prioritizing mobile orders. Encourage midday traffic with "Afternoon Specials" discounts between 1-3 PM and interactive events or product demos around 2 PM. Engage the local community by offering exclusive deals for students and nearby businesses during slower afternoon hours.

- Hell's Kitchen: Optimize morning operations with faster checkout and mobile order priority from 9-10 AM. Draw in evening customers with "8 PM Happy Hour" discounts or "Last-Minute Shopper" deals, and host engaging pop-up events or live music to create a lively atmosphere. Collaborate with nearby dining spots to offer paired discounts for customers heading home from work or dinner.

- Lower Manhattan: Maximize commuter sales with extended morning promotions from 6-10 AM. Attract post-work shoppers with "Twilight Discounts" from 5-7 PM, and address low late-evening sales by considering earlier closing hours. Strengthen partnerships with local businesses for joint promotions, such as discounts on coffee or snacks during quieter hours.

***Focus on Bestsellers and Improve Low-Demand Items***

Since coffee, tea, and bakery items drive the most sales across all locations, Maven Roasters could introduce combo deals or loyalty rewards to encourage repeat purchases. Meanwhile, low sales of packaged chocolate and branded merchandise suggest a need for better placement, promotions, or bundling with popular items to boost visibility. Testing limited-time offers or seasonal packaging might also help attract more interest in these slower-moving products.

***Drive Revenue with Top-Performing Products  and Manage Low-Demand Items***

- Astoria: Build on Brewed Chai Tea's strong performance by promoting it with loyalty perks such as "Buy 5, Get 1 Free" to keep customers engaged. Encourage sales for Barista Espresso, which has lower volume but high revenue, by emphasizing its high-quality beans or introducing limited-edition variations. Increase demand for syrups by bundling sugar-free and regular options with popular drinks or offering free flavor shots for a limited time.

- Hell’s Kitchen: Make the most of Brewed Chai Tea's success by offering seasonal variations like chai latte specials to keep customers excited. Find ways to boost revenue for Gourmet Brewed Coffee by testing premium pricing or promoting larger sizes. Help customers personalize their drinks by highlighting syrups as customization options and featuring them on digital menu boards or apps.

- Lower Manhattan: Take advantage of Barista Espresso's popularity by introducing loyalty-based incentives, specialty versions, or subscription-based coffee programs. Focus on increasing Brewed Chai Tea sales by marketing it as a specialty item and offering premium add-ons like oat milk or honey drizzle. Encourage more purchases of Brewed Green Tea and syrups with wellness-focused promotions like "Antioxidant Boost" bundles or limited-time flavors.

## Limitations

1. Short Time Frame – This analysis covers only six months (January to June 2023), so it may not fully capture seasonal trends or long-term shifts in customer behavior. A full year of data would provide a more complete picture of patterns and opportunities.

2. No Customer-Level Insights – The dataset is transaction-based, meaning it doesn’t track individual customers, which are typically analyzed to understand repeat purchases, customer loyalty, and personalized buying habits, all of which could help in shaping targeted marketing strategies.

3. External Factors Not Considered – The analysis focuses on sales data without factoring in outside influences like local events, competitor activity, or economic trends. These factors may have played a role in sales fluctuations but aren't reflected in the dataset.
