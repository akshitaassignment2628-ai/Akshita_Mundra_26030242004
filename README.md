# T03 – Inventory Reorder Alert Tool

**Student:** Akshita Mundra  
**Task ID:** T03  
**Theme:** A. No-code apps & dashboards

## What this project does
- Calculates Safety Stock, Reorder Point (ROP), EOQ and Days of Stock Left for 150 SKUs.
- Flags SKUs whose current stock is below calculated ROP.
- Generates a recommended purchase quantity.
- Provides a warehouse-manager purchase list.
- Gives Top 5 High Priority list of SKUs that need to be ordered for every filter.
- Shows dynamic requirements and budgets.

## Calculation assumptions
- Service level: approximately 90%; Z = 1.65.
- Demand standard deviation is treated as daily demand standard deviation.
- Annual demand = average daily demand × 365.
- Annual holding cost per unit = unit cost × annual holding cost rate.
- Reorder flag: current stock < calculated ROP.
- Recommended order quantity for flagged SKUs = max(ceil(EOQ), ceil(ROP − current stock)); otherwise 0.

## Files
- `T03_Inventory_reorder_alert_tool.xlsx` – calculations, formula explanation, manual verification and purchase list.
- `T03_Inventory_Reorder_HTML_Dashboard` – live browser dashboard/app.

