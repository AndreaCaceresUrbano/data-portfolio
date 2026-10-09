# Retail Sales Analysis

End-to-end retail analytics project using Python, Power BI, DAX and Tabular Editor.

The objective of this project is to clean and prepare retail transaction data with Python and build an interactive Power BI dashboard to analyze sales performance, customers and shopping malls.

## Technologies

- Python
- Pandas
- Power BI
- DAX
- Power Query
- Tabular Editor

## Project Workflow

1. Data cleaning and validation with Python
2. Data preparation for Power BI
3. Data modeling in Power BI
4. Calendar table creation
5. Core KPI measures
6. Time Intelligence using Calculation Groups
7. Dynamic ranking using DAX
8. Interactive dashboard development

## Dynamic Ranking

A dynamic ranking pattern was implemented in DAX to rank shopping malls by total sales.

The ranking updates automatically according to the filters applied in the report, such as year, category or gender.

### DAX measure

```DAX
Mall Rank =
IF(
    ISINSCOPE(customer_shopping_data_clean[shopping_mall]),

    VAR CurrentSales =
        [Total Sales]

    VAR Ranking =
        RANKX(
            ALLSELECTED(customer_shopping_data_clean[shopping_mall]),
            [Total Sales],
            ,
            DESC,
            DENSE
        )

    RETURN
        IF(
            NOT ISBLANK(CurrentSales),
            Ranking
        )
)
```

## Status

Project in progress.
