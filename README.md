# Olist-Sales-Analysis

Olist is an Ecommerce site based in Brazil. Based on data from the years 2016-2018, analysis was conducted to gain insight on sales metrics to further understand product and category performance, order patterns and return metrics. Using this information, future decisions were guided towards expanding into new markets, pushing underperforming products and categories and overall maximising revenue.  

# Table of Contents

- [Objectives](#Objectives)
- [Data Description](#Data_Description)
- [Data Structure & Initial Checks](#Data_Structure_&_Initial_Checks)
- [Executive Summary](#Executive_Summary)
- [Insights Deep Dive](#Insights_Deep_Dive)
  - [Orders/Shipping](#Orders/Shipping)
  - [Categories](#Categories)
  - [Customers](#Customers)
- [Recommendations](#Recommendations)
- [Assumptions and Caveats](#Assumptions_and_Caveats)

## Objectives
Order and Shipping Analysis: To assess overall trends related to orders, revenue and shipping
Categorical Insights: To investigates patterns in product categories related to sales and growth 
Customer and Geographical Profiling: To analyse customer behaviour and geographical data  

## Data Description
The analysis is based on a rich dataset encompassing several key aspects to the Olist business operations.
1. Customer Details
2. Order Details
3. Product Details
4. Geographical Details
The use of customer, order, product and geographical data allows for meaningful insights to be drawn and make data-driven decisions to enhance business strategy and operations. By focusing on these key areas, improvements will be seen in optimised product offerings,  customer reach, retention rate, and drive sustainable growth.

The SQL queries used to inspect and clean the data for this analysis can be found [here](assets/Queries/SQL/)

DAX measures used in power query can be found [here](assets/Queries/DAX/)

## Data Structure & Initial Checks
The company's main database structure as seen below consists of nine tables with a total row count of 17094341 records. A description of each table is as follows:
[Entity Relationship Diagram here](assets/ERD/)

## Executive Summary

Findings indicate steady growth in revenue and orders with a peak in November 2017(__), before plateauing at around February 2018. The best overall performing categories are bed, table and bath; computer accessories and beauty/health. Most customers are based in the three biggest states, Rio de Janeiro(13%), Minas Gerais (11%) and São paulo (38%). Furthermore, following states order patterns shows that many of the highest purchasing states spend less on average per order while the inverse happens the lowest purchasing states. Moreover, there is also a correlation between delivery times as the states that order the most spend the least on shipping costs and have the fastest delivery times again the inverse happens. 

Freight/shipping prices had a significant rise after February 2018 peaking at __ in $22.95 in July of that year. This rise also occurred during the revenue plateau, suggesting correlation between the two factors. In fact, we can see by the line chart that payments made by credit card really took the majority place on brazilian e-commerce. Besides that, from 201803 it's possible to see a little decrease in this type of payment. By the other hand, payments made by debit card are showing a growing trend since 201805, which is a good opportunity for investors to improve services for payments like this.
On the bar chart above, we can see how Brazilian customers prefer to pay the orders: mostly of them pay once into 1 installment and it's worth pointing out the quantity of payments done by 10 installments.
[Visualisation, including a graph of overall trends or snapshot of a dashboard]

At Olist, understanding the market dynamics and performance metrics is crucial to driving company growth and sustainability. This report provides an in-depth analysis about order and shipping metrics, category insights and customer ___. By analysing these insights, areas of success and further potential improvement can be identified. 

## Insights Deep Dive

### Orders/Shipping
Overall, between October 2016 and August 2018 Olist experienced rapid growth, peaking in November at $238 million before plateauing through 2018 next year at around $200 - 210 million. During this same time freight prices grew rapidly after February 2018 from an average of $18 to $22. Two significant peaks for shipping times, December 2017 due to busy holiday season and Feb/Mar 2018 which was caused by postal strikes that happened in areas of Brazil. Dig down, the peak time that consumers are more likely to make orders is in the afternoon of all weekdays, especially Monday to Wednesday.

[Visualization specific to category 1]

### Categories
The company is not over reliant on any singular category as no one category takes up over 15% of total order; bad, bath and table , computer accessories and health & beauty, and have the most. Most revenue comes from the top 25 categories, showing that Olist has a diversified portfolio of products. Categories such as construction tools (34.80%), construction tools light(37.72%), bedroom furniture(24.41%) and pets(15.15%) have seen the biggest growth in the first three quarters of 2018. Meanwhile, categories such as fashion underwear beach (21.78%), garden tools (13.13%). Overall, many categories in terms of being a consistent source of revenue which is represent in the annual growth rate of 1.23% for revenue and 1.05% for orders


[Visualization specific to category 2]

### Customers
An average monetary customer is $136 and 75% of the customers spend less than $150 and the maximum was $4690. Furthermore, the average customer spends $136 and 75% spend less than $150. Only 3% of customers purchased more than once. Most customers are located on the east coast, in cities such as Sao Paulo and Rio de Janeiro. Not only is this where most of the population live but these areas have the fastest shipping and the lowest cost of shipping. This makes sense as these places have the most infrastructure. Furthermore, the low cost is enticing for people in this region. However, there is untapped potential in the country north-east with areas such as Ceara, Pernambuco and Para as these areas have a low amount of orders compared to their population.


[Visualization specific to category 3]

## Recommendations
Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following:
Focus on pushing products in categories that showed high growth such as construction tools, pets and bedroom furniture. This will help to grow revenue and would enable the company to enhance its overall performance and mitigate potential risks in the market.
Expand into the underperforming regions of Ceara, Pernambuco and Para to increase customer base. 
Only 3% of customers are repeat customers. Improving this number is crucial to making revenue more stable. Offer more deals and advertise sales to previous customers to retain sales.
Consider promotion at busy times such as holiday period and black Friday to increase volume or launch new products.

## Assumptions and Caveats
Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:
Assumption 1 (ex: missing country records were for customers based in the US, and were re-coded to be US citizens)


Assumption 1 (ex: data for December 2021 was missing - this was imputed using a combination of historical trends and December 2020 data)


Assumption 1 (ex: because 3% of the refund date column contained non-sensical dates, these were excluded from the analysis)
