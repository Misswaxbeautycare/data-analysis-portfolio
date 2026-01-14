# Simple Sales Analysis Demo
# Author: Miss Nyunge

import pandas as pd

# Create simple sales data
data = {
    "Product": ["Product A", "Product B", "Product C", "Product D"],
    "Revenue": [1200, 900, 1500, 700]
}

# Create DataFrame
df = pd.DataFrame(data)

# Display data
df

# Total revenue
total_revenue = df["Revenue"].sum()
total_revenue

# Best selling product
best_product = df.loc[df["Revenue"].idxmax()]
best_product
