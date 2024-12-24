Average Delivery Time
```dax
AVERAGEX(
    'Ecom',
    DATEDIFF(
        'Ecom'[order_purchase_timestamp],
        'Ecom'[order_delivered_customer_date],
        DAY
    ))
```

Montly Orders 
```dax
COUNT(Ecom[order_id])
```

Monthly Revenue
```dax
SUM(Ecom[payment_value])
```

Previous Monthly Revenue
```dax
Previous Monthly Order = CALCULATE([Monthly Orders], DATEADD(dDate[Date], -1 , MONTH))
```

Previous Month Revenue 
```dax
CALCULATE([Monthly Revenue],DATEADD(dDate[Date], -1, MONTH))
```
Order Growth Rate 
```dax
 DIVIDE([Monthly Orders] - [Previous Monthly Order], [Previous Monthly Order])
```

Retention Rate 
```dax
DIVIDE(COUNTROWS(FILTER(SUMMARIZE(Ecom, Ecom[customer_id], "Order Count", COUNT(Ecom[order_id])),[Order Count] > 1)),
COUNT(Ecom[customer_id]), 0) * 100
```

Revenue Growth Rate 
```dax
DIVIDE([Monthly Revenue] - [Previous Month Revenue], [Previous Month Revenue]) 
```

