# DAX Measures - Sales Dashboard

Aşağıdakı ölçüləri Power BI-də Measures table-ə əlavə edin.

## Əsas KPI-lər

```dax
Total Sales = SUM(sales_data[SalesAmount])
```

```dax
Total Cost = SUM(sales_data[Cost])
```

```dax
Total Profit = [Total Sales] - [Total Cost]
```

```dax
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
```

```dax
Total Orders = DISTINCTCOUNT(sales_data[OrderID])
```

```dax
Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)
```

```dax
Total Quantity = SUM(sales_data[Quantity])
```

## Time Intelligence

```dax
Sales YTD = TOTALYTD([Total Sales], 'Date'[Date])
```

```dax
Sales Previous Year = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))
```

```dax
YoY Growth % = DIVIDE([Total Sales] - [Sales Previous Year], [Sales Previous Year], 0)
```

## Digər faydalı ölçülər

```dax
Discount Impact = SUMX(sales_data, sales_data[Quantity] * sales_data[UnitPrice] * sales_data[Discount%] / 100)
```

```dax
Avg Discount % = AVERAGE(sales_data[Discount%])
```

Qeyd: Date table yaratmağı unutmayın. Calendar table üçün Power Query və ya DAX ilə yarada bilərsiniz.
