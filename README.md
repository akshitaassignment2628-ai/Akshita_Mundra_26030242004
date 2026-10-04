# T03 – Inventory Reorder Alert Tool

**Student:** Akshita Mundra  
**Task ID:** T03  
**Theme:** A. No-code apps & dashboards

## What this project does
- Calculates Safety Stock, Reorder Point (ROP), EOQ and Days of Stock Left for 150 SKUs.
- Flags SKUs whose current stock is below calculated ROP.
- Generates a recommended purchase quantity.
- Provides a 10-SKU manual verification sheet.
- Provides a warehouse-manager purchase list.
- Includes an AI-use-log template with 15 prompts.

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
- Original workbook is the supplied input file.

## GitHub Pages
Upload the HTML file to a GitHub repository and enable GitHub Pages from the repository's Settings → Pages. The resulting Pages URL can be submitted as the project link.

## Important
The purchase list is a planning recommendation based on the stated assumptions; the warehouse manager should confirm supplier constraints, minimum order quantities, budgets and current operational conditions before ordering.
