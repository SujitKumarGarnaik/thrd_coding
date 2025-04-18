
This Python script price.py dynamically adjusts product prices based on inventory and recent sales data. It applies tiered pricing rules and ensures minimum profit margins.


- products.csv – Product catalog with price, cost, and stock.
- sales.csv – Quantity sold per product in the last 30 days.
- updated_prices.csv – Output with new calculated prices.
- price.py – Script to compute new prices.

## How It Works

1. Merges product and sales data using SKU.
2. Applies pricing rules in the given priority order:
   - Low stock & high demand → +15%
   - Dead stock → −30%
   - Overstocked → −10%
3. Ensures minimum price = 120% of cost price.
4. Outputs final price rounded to 2 decimals and includes unit (INR).

## Dependencies

- Python 3
- pandas pip install pandas

## Run

## bash
python price.py
