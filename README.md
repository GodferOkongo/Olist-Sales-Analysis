# Olist-Sales-Analysis

Olist is an Ecommerce site based in Brazil. Based on data from the years 2016-2018, analysis was conducted to gain insight on sales metrics to further understand product and category performance, order patterns and return metrics. Using this information, future decisions were guided towards expanding into new markets, finding and pushing underutilised products and categories and overall maximising revenue.  

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
1. Customer Details: This data provides insight into customers, including trends that relate to payment types, average amount spent and when purchases are made. This information can be used to better understand customer trends to further to improve their ecommerce experience.
   
2. Order Details: This data provides comprehensive information about the orders placed. Seller information, Shipping times and costs, dates and quantities. It help tracking purchasing patterns and identify not only high-performing products, but products with high growth.
   
3. Product Details: This data sets includes information about each product. Categories, price and sales performance. This allows for evalution for what products and categories are the most popular and profitable.
   
4. Geographical Details: Geogrpahical data that details the regions of customers and sellers. this helps evaluates regional performance and tailor maketing strategies to different areas.
   
The use of customer, order, product and geographical data allows for meaningful insights to be drawn and make data-driven decisions to enhance business strategy and operations. By focusing on these key areas, improvements will be seen in optimised product offerings, customer reach, retention rate, and drive sustainable growth.

The SQL queries used to inspect and clean the data for this analysis can be found [here](assets/Queries/SQL/)

DAX measures used in power query can be found [here](assets/Queries/DAX/)

## Data Structure & Initial Checks
The company's main database structure as seen below consists of nine tables with a total row count of 17,094,341 records. A description of each table is as follows:
[Entity Relationship Diagram here](assets/ERD/)

## Executive Summary

Findings indicate steady growth in revenue and orders with a peak in November 2017 of $238 million, before plateauing at around February 2018 averaging around $200 million. The best overall performing categories are bed, table and bath; computer accessories and beauty/health. Most customers are based in the three biggest states, Rio de Janeiro(13%), Minas Gerais (11%) and São paulo (38%). Furthermore, order patterns shows that many of the highest purchasing states spend less on average per order while the inverse happens the lowest purchasing states. Moreover, there is also a correlation between delivery times as the states that order the most spend the least on shipping costs and have the fastest delivery times and again the inverse is also illustrated with states the order the least. Freight/shipping prices had a significant rise after February 2018 peaking at $22.45 in July of that year. This rise also occurred during the revenue plateau, suggesting correlation between the two factors. 

At Olist, understanding the market dynamics and performance metrics is crucial to driving company growth and sustainability. This report provides an in-depth analysis about order and shipping metrics, category and customer insights. By analysing these findings, areas of success and further potential improvement can be identified. 

## Insights Deep Dive

### Orders/Shipping
Overall, between October 2016 and August 2018 Olist experienced rapid growth, peaking in November at $238 million before plateauing through 2018 next year at around $200 - 210 million. During this same time freight prices grew rapidly after February 2018 from an average of $18 to $22. Two significant peaks for shipping times, December 2017 due to busy holiday season and Feb/Mar 2018 which was caused by postal strikes that happened in areas of Brazil. Most customers are located on the east coast, in cities such as Sao Paulo and Rio de Janeiro. Not only is this where most of the population live but these areas have the fastest shipping and the lowest cost of shipping. This makes sense as these places have the most infrastructure. Furthermore, the low cost is enticing for people in this region. However, there is untapped potential in the country north-east with areas such as Ceara, Pernambuco and Para as these areas have a low amount of orders compared to their population. 

![Ordrers_&_Shipping]()


### Customers
An average monetary customer spends $136 and 75% spend less than $150. Transitioning to payment types now, credit card really took the majority place on brazilian e-commerce with 73% of purchases being made with that payment type. Besides that, from March 2018 it's possible to see a little decrease in this type of payment. By the other hand, payments made by debit card are showing a growing trend since may 2018, which is a good opportunity for investors to improve services for payments like this. Additionally, Brazilian customers prefer to pay the order in one installment. Though, over one million orders had payments with 10 or more installments and further 10 out of 11 of the most expensive average payment installments were double digit, showing that customers a very willing to use long-term installments to pay for expensive orders. Dig down, the peak time that consumers are more likely to make orders is in the afternoon of all weekdays, especially Monday to Wednesday.

[Visualization specific to category 2]

### Categories
The company is not over reliant on any singular category as no one category takes up over 15% of total order. The top 3 categories in terms of orders are bed, bath and table, computer accessories and health & beauty. Most revenue comes from the top 25 categories, showing that Olist has a diversified portfolio of products. Moreover, Categories such as construction tools (34.80%), construction tools light(37.72%), bedroom furniture(24.41%) and pets(15.15%) have seen the biggest growth in revenue in the first three quarters of 2018. Meanwhile, categories like fashion underwear beach (21.78%), garden tools (13.13%) have had the biggest growth in terms of orders in the same time period. 

However, 47% of categories have shown negative revenue growth rate. Most categories perform inconsistantly which is only compounded by the low amount of repeat purchases, contributing to low annual growth rate of 1.23% for Olist. While there are some bright spots, more has to be done to drive more traffic to the site and create loyal customers. 

[Visualization specific to category 3]

## Conclusion
-Expand customer base into untapped and underperforming markets
-Push deals and offers to increase organic traffic
-Enhance product visability
-Improve customer retention


## Recommendations
1. Expand customer base into untapped and underperforming markets
Focus on increasing sales in regions that have tradionally performed poorly relative to their potential such as Ceara, Pernambuco and Para by leveraging successful strategies from higher performing regions and increasing promotion.

2. Increase Deals and Offers for more Organic Traffic
Busy events such as the holiday period, Black Friday should involve more promotional deals. Furthermore, intice customers to use more payment installments and pushing categories with high growth. Plan high-demand periods with additional logistical support to prevent delays.

3.Enhance Product Visability
Improve product recommendations and search visibility to high growth categories such as construction tools, bedroom furniture and pets.

4. Improve Customer Retention
Encourage repeat purchases by offering incentives such as discounts.

    
###
Link to Dashboards
