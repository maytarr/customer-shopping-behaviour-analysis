# Customer Shopping Behaviour Analysis

An end-to-end analysis of 3,900 retail purchases: cleaning the data in Python, answering business questions with SQL in PostgreSQL, and presenting the results in a Power BI dashboard and a slide deck.

Based on [Amlan Mohanty's data analyst portfolio project tutorial](https://www.youtube.com/watch?v=5PrZvPeUw60).

## Business questions

1. What is the total revenue from male vs. female customers?
2. Which customers used a discount but still spent more than the average purchase?
3. Which 5 products have the highest average review rating?
4. How do average purchase amounts compare between Standard and Express shipping?
5. Do subscribed customers spend more than non-subscribers?
6. Which 5 products have the highest share of purchases with a discount?
7. How do customers split into New, Returning and Loyal segments?
8. What are the top 3 most purchased products in each category?
9. Are repeat buyers (more than 5 previous purchases) more likely to subscribe?

## Tools

- **Python** (Pandas) for cleaning and preparing the data
- **PostgreSQL** for the analysis (CTEs, subqueries, CASE logic, window functions)
- **Power BI** for the dashboard
- **PowerPoint** for the stakeholder presentation

## Files

| File | What it is |
|---|---|
| `customer_shopping_behavior.csv` | The raw dataset |
| `customer_shopping_behavior_analysis.ipynb` | Data cleaning in Python, then loading into PostgreSQL |
| `SQL/customer_behavior_analysis.sql` | The SQL queries answering each business question |
| `powerbi/customer_behaviour_dashboard.pbix` | Power BI dashboard |
| `powerpresentation/Customer-Shopping-Behavior-Analysis.pdf` | Presentation of the findings (also as `.pptx`) |

## Running it

1. Install dependencies with [uv](https://docs.astral.sh/uv/): `uv sync`
2. Create a PostgreSQL database called `customer_behavior`
3. Set your database password as an environment variable, e.g. in PowerShell: `$env:PGPASSWORD = "your password"`
4. Run the notebook, then the queries in `SQL/`
