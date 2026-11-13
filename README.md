# Analyzing_Motorcycle_Part_Sales
Derived insights about motorcycle part sales over time across multiple warehouse sites

## Motorcycle Parts Revenue Analysis: Wholesale Net Revenue by Product, Month & Warehouse | SQL, PostgreSQL

Wrote a PostgreSQL query that breaks wholesale net revenue down by product line, month and warehouse, so a board of directors can see which products and locations drive revenue and how that shifts from June to August 2021.

# CONTEXT
A motorcycle parts seller with three warehouses, retail and wholesale channels and three payment methods (each with its own fee) wanted to understand wholesale revenue in detail.

# MY ROLE
I designed and wrote the query and checked its output.

# WHAT I DID
• Filtered orders to the Wholesale client type
• Converted order dates into readable month names (June, July, August) using EXTRACT and CASE
• Calculated net revenue per group as total sales minus payment fees
• Grouped by product line, warehouse and month, and sorted by product line, month and net revenue (highest first) for easy reading

# RESULTS
• A 48-row table in the format product_line | month | warehouse | net_revenue
• Top finding: Engine product line in Central warehouse had the highest net revenue in August ($9528.71)
•  Bottom finding: Electrical system product line in West warehouse had the lowest net revenue in July ($449.46)

# TECH STACK
SQL, PostgreSQL, CASE expressions, aggregate functions (SUM), GROUP BY and ORDER BY
