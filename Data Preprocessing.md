## Data Preprocessing

**Current workflow**  
I preprocess the raw event data in Python to build a slimmed-down data mart for local visualization and analysis.

1. **Create Order & Log Tables**  
2. **Common preprocessing steps**  
   - Remove all rows where `price` ≤ 0  
   - Replace nulls in `brand` with `"unknown"`  
   - Drop rows where `user_session` is null  
   - Drop the `category_code` column  
3. **Order table**  
   - Keep only rows with `event_type == "purchase"`  
4. **Log table**  
   - Retain only these columns:  
     `event_time`, `event_type`, `brand`, `user_id`, `user_session`

### Python code

```python
# 1. Remove rows with non-positive price
df_all = df_all[df_all['price'] > 0].copy()

# 2. Fill nulls in 'brand' with 'unknown'
df_all['brand'] = df_all['brand'].fillna('unknown')

# 3. Drop rows where 'user_session' is null
df_all = df_all.dropna(subset=['user_session'])

# 4. Drop the 'category_code' column
df_all = df_all.drop(columns=['category_code'])

# Split into orders and logs
orders = df_all[df_all['event_type'] == 'purchase'].copy()

logs = df_all[[
    'event_time',
    'event_type',
    'brand',
    'user_id',
    'user_session'
]].copy()
