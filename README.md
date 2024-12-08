# Pizza-Sales-Analysis_SQL
# Overview
The objective of this project was to perform a comprehensive analysis of a pizza sales dataset for a database. The project utilized SQL to analyze sales trends, customer preferences, and revenue patterns, offering valuable insights into business performance. This analysis involved creating and querying relational database tables to extract meaningful patterns and key business metrics.

# 1. Database and Table Setup
A relational database named dominos was created to store data related to orders, order details, and pizza specifications.
Tables Created:
orders: Contains metadata about each order, such as order ID, date, and time.
order_details: Includes detailed information about pizzas ordered, such as pizza ID, order ID, and quantity.


# 2. Business Questions and Analysis
   
Q1: Total Number of Orders Placed
Objective: Calculate the total number of orders in the database.
Result: Aggregated the orders table to determine the total order count.

Q2: Total Revenue Generated
Objective: Calculate total revenue from pizza sales.
Result: Used a join between order_details and pizzas tables to multiply the quantity of pizzas ordered by their prices, summing the results.

Q3: Highest-Priced Pizza
Objective: Identify the pizza with the highest price.
Result: Joined pizza_types and pizzas tables, sorted prices in descending order, and retrieved the top entry.

Q4: Most Common Pizza Size Ordered
Objective: Determine the most popular pizza size.
Result: Counted orders grouped by size and sorted results to identify the size with the highest frequency.

Q5: Top 5 Most Ordered Pizza Types
Objective: Identify the five most frequently ordered pizza types.
Result: Summed order quantities grouped by pizza type and sorted results in descending order to fetch the top 5.

Q6: Total Quantity of Each Pizza Category Ordered
Objective: Calculate the total quantity ordered for each pizza category.
Result: Aggregated quantities grouped by pizza category.

Q7: Distribution of Orders by Hour
Objective: Understand ordering trends across different hours of the day.
Result: Grouped orders by the hour of the order_time and counted the number of orders.

Q8: Average Pizzas Ordered Per Day
Objective: Calculate the average number of pizzas ordered daily.
Result: Grouped orders by date and computed the average across all days.

Q9: Top 3 Most Ordered Pizza Types Based on Revenue
Objective: Identify the top 3 pizza types that generated the most revenue.
Result: Multiplied pizza quantity by price, grouped by pizza type, and sorted results to fetch the top 3.

Q10: Percentage Contribution to Total Revenue
Objective: Analyze the revenue contribution of each pizza category as a percentage of the total.
Result: Divided category-wise revenue by total revenue and multiplied by 100 to calculate percentage contributions.

Q11: Cumulative Revenue Over Time
Objective: Track the cumulative revenue generated over time.
Result: Summed daily revenues in chronological order using a window function.

Q12: Top 3 Most Ordered Pizza Types by Revenue for Each Category
Objective: Rank pizza types within each category based on revenue and identify the top 3 for each.
Result: Used window functions to rank pizzas within categories and filtered results for the top 3.


