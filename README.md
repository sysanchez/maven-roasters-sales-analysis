# Maven Roasters Sales Analysis (Jan 2023 - June 2023)

## Key Sections

  - [Background and Overview](Background-and-Overview)
  - [Data Structure Overview](Data-Structure-Overview)
  - [Executive Summary](Executive-Summary)
  - [Deep-dive Insights](Deep-dive-Insights)
  - [Recommendations](Recommendations)
## Background and Overview: 
Maven Roasters is a coffee shop chain with three locations in New York City: Astoria, Hell’s Kitchen, and Lower Manhattan.

This analysis was made to help identify bestselling products, peak transaction times, and revenue drivers across Maven Roasters’ three NYC locations to help the  owner understand purchase behavior, identify patterns, trends and opportunities for the business and streamline operations.

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

The dataset is available here.

Data dictionary is provided here.

## Executive Summary

From January to June, sales across the three Maven Roasters locations followed an upward trend, peaking in June with each store generating more than $50,000 in revenue. February saw a slight decline in all stores, possibly due to lower post-holiday consumer spending or seasonal fluctuations in customer traffic with revenue dropping to $2,209 in Astoria, $2,101 in Hell's Kitchen, and $1,223 in Lower Manhattan..

The busiest days vary by store, but weekdays generally see the highest number of transactions. In Astoria, Thursday has the most transactions (7,427), followed closely by Monday (7,403) and Wednesday (7,370). Hell's Kitchen sees the highest transaction volumes on Friday (7,489) and Tuesday (7,572), while in Lower Manhattan, Monday is the busiest day (7,136).

Coffee is the best-selling category across all stores, with 20,025 transactions in Astoria, 20,187 in Hell’s Kitchen, and 18,204 in Lower Manhattan. Barista Espresso leads in both transactions and revenue in Hell’s Kitchen (6,153 transactions, $32,420 revenue) and Lower Manhattan (5,320 transactions, $31,051 revenue). In contrast, Astoria’s top-selling item is Brewed Chai Tea, generating 6,293 transactions and $27,428 in revenue. Syrups (regular and sugar-free) had the lowest sales across all stores, with total transactions ranging from around 400 to 2,100 and revenue between $450 and $2,600, indicating they are primarily add-ons rather than standalone purchases

Below is a screenshot of the dashboard in Excel. The entire interactive dashboard can be downloaded here.

## Deep-dive Insights

### Astoria

**Sales Trends Over Time**

Total revenue showed steady growth, increasing from $27,314 in January to $55,083 in June, reflecting a 101% increase over six months. There was a slight dip in February, likely due to post-holiday spending slowdowns, but things picked up again in March and continued to grow. June marked the highest revenue, likely driven by increased customer demand or seasonal trends.

**Busiest Days of the Week & Busiest Hours of the Day**

Transactions vary throughout the week, with the highest activity on Thursday (7,427transactions) and the lowest on Saturday (6,942 transactions). Monday, Wednesday, and Friday see strong sales with over 7,000 transactions, while weekend transactions are lower, likely due to lower foot traffic on Saturdays and Sundays.

The busiest time of the day is between 9 AM and 10 AM, with transactions exceeding 5,000. After 11 AM, sales drop to around 3,000 per hour and remain steady throughout the afternoon. This trend suggests high demand for morning coffee, while afternoon sales remain consistent but lower

**Product Performance & Revenue Drivers**

Coffee is the best-selling product category, with 20,025 transactions, followed closely by tea at 16,260. Bakery items also see strong sales, with more than 7,289 transactions, while categories like packaged chocolate and branded merchandise have significantly lower sales, with fewer than 400 transactions each. This suggests that customers primarily visit for beverages, with food as a secondary purchase, while packaged retail items see limited demand.

Brewed Chai Tea leads in transactions with over 6,200 sales, generating nearly $27,500 in revenue, while Barista Espresso, despite having fewer transactions (4,930), brings in a similar amount of revenue. Regular and sugar-free syrups have the lowest sales, with fewer than 1,200 combined transactions and under $2,000 in revenue, reinforcing their role as add-ons rather than primary purchases. Overall, brewed beverages dominate both sales and revenue, highlighting customer preference for handcrafted drinks.

### Hell’s Kitchen

**Sales Trends Over Time**

Total revenue steadily increased over six months, with a small dip of $2,101 in February before reaching $56,957 in June. The most significant growth occurred between April and May, with an increase of over $12,000, possibly driven by seasonal demand, marketing efforts, or higher customer traffic.

**Busiest Days of the Week & Busiest Hours of the Day**

Tuesday and Friday saw the highest number of transactions, with 7,472 and 7,489, respectively, indicating strong midweek and end-of-week sales. Saturday had the lowest transaction count at 6,846, suggesting a slight dip in weekend activity. Overall, transactions remained fairly consistent throughout the week.

Transactions peak in the morning, with the highest volume at 9 AM (6,909 transactions) and 10 AM (6,767 transactions), highlighting strong demand during early hours. Activity gradually declines throughout the day, with the lowest number of transactions recorded at 8 PM (528). This suggests that most customers visit earlier in the day, likely for their morning coffee or breakfast.

**Product Performance & Revenue Drivers**

Coffee leads in sales with 20,187 transactions, followed by bakery items with 7,617 and drinking chocolate with 3,763, while other categories see lower demand. Branded products (119 transactions) and packaged chocolate (197 transactions) have the fewest sales, suggesting they appeal to a smaller, niche customer base.

Barista Espresso leads in revenue, generating $32,420 from 6,153 transactions, showing strong customer preference for premium coffee options. Brewed Chai Tea follows closely with $25,645 in revenue, despite slightly fewer transactions at 5,824, indicating higher pricing or larger order sizes. In contrast, sugar-free syrup has the lowest revenue at just $718 from 602 transactions, suggesting limited demand for specialty add-ons.

### Lower Manhattan

**Sales Trends Over Time**

Revenue showed a strong upward trend, increasing from $26,543 in January to $54,446 in June, more than doubling over six months. The most significant jump occurred between April and May, with a $12,541 increase, suggesting higher customer demand or successful business strategies. This consistent growth highlighted strong performance momentum and potential for further expansion.

**Busiest Days of the Week & Busiest Hours of the Day**

Monday is the busiest day of the week, with 7,136 transactions, slightly ahead of Thursday at 6,920. Weekday transactions remain fairly consistent, while weekends see a small dip, with Saturday (6,722) and Sunday (6,679) having the lowest activity. This suggests that customer traffic is higher during the workweek, potentially due to routine coffee runs or office-related purchases.

Morning hours are the busiest, with transactions peaking around 10 AM at over 6,000. The early rush begins at 6 AM and remains strong through 9 AM, likely driven by commuters and morning routines. After 11 AM, transactions drop significantly and gradually decline through the afternoon, with minimal activity after 6 PM.

**Product Performance & Revenue Drivers**

Coffee is the top-selling category with 18,204 purchases, surpassing tea at 13,912. Bakery items follow with 7,890 transactions, making them the top non-beverage choice. Meanwhile, niche products like packaged chocolate (180) and branded items (349) have the lowest sales, indicating a smaller customer base.

Barista Espresso leads in both transactions (5,320) and revenue ($31,051), making it the top-performing product. Gourmet brewed coffee and brewed chai tea also drive strong sales, generating over $23,000 each. Meanwhile, sugar-free syrup has the lowest figures, with only 830 transactions and $1,153 in revenue, indicating lower demand compared to core beverage offerings.

## Recommendations

Based on the key insights identified, the following recommendations are proposed.

***Boost Sales Consistency with Seasonal Strategies***

To keep sales growing and avoid seasonal dips like February, Maven Roasters could run limited-time promotions or special events to attract more customers. Adjusting marketing strategies based on each location’s traffic patterns might also help smooth out slower months.

***Maximize Weekday Sales and Boost Weekend Traffic*** 

To make the most of peak weekday traffic, Maven Roasters could offer targeted promotions or loyalty incentives on these high-traffic days to boost sales further. Additionally, exploring ways to drive more weekend transactions—such as special weekend-exclusive menu items or discounts—could help balance sales across the week.

***Optimize Store Hours and Promotions for Peak and Slow Periods***

To maximize sales, Maven Roasters could introduce morning promotions or loyalty incentives to encourage repeat visits during peak hours. Since transactions drop off in the afternoon and evening, offering targeted discounts or new product options later in the day may help attract more customers during slower periods. For the hours with minimal to no activity, adjusting store hours to better align with customer demand or exploring alternative revenue streams, such as online orders or special evening events, could help optimize operations.

***Focus on Bestsellers and Improve Low-Demand Items***

Since coffee, tea, and bakery items drive the most sales across all locations, Maven Roasters could introduce combo deals or loyalty rewards to encourage repeat purchases. Meanwhile, low sales of packaged chocolate and branded merchandise suggest a need for better placement, promotions, or bundling with popular items to boost visibility. Testing limited-time offers or seasonal packaging might also help attract more interest in these slower-moving products.

***Drive Revenue with Top-Performing Products  and Manage Low-Demand Items***

Maven Roasters should continue promoting high-performing drinks like Barista Espresso and Brewed Chai Tea, as they generate strong revenue despite varying transaction counts. To increase sales of lower-demand items like syrups, the company could bundle them with popular drinks or offer limited-time flavors to encourage add-on purchases. Additionally, highlighting handcrafted beverages in marketing efforts can reinforce customer preference and further boost sales.
