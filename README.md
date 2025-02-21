# Energy-Consumption-Dashboard

📊 Project Overview

The Energy Consumption Dashboard is a comprehensive analytical tool built using Power BI to visualize and analyze energy consumption data across different cities, countries, and energy types (Electricity, Gas, Water). The dashboard helps stakeholders gain insights into consumption patterns, costs, and key performance indicators (KPIs).

🛠️ Project Features

4 Dashboard Pages:

Overview: Displays overall energy consumption trends across all types and regions.

Electricity: Detailed analysis of electricity consumption.

Gas: Focused insights on gas consumption.

Water: Visualization of water consumption data.

DAX Measures:

-- Units Consumed
Units Consumed = SUM('Energy consumptions'[Units])

-- Total Cost
Total Cost = SUMX(
    'Energy consumptions',
    'Energy consumptions'[Units] * RELATED(rates[Price per Unit])
)

KPI Cards: Key metrics on each page displaying total cost and units consumed.

Slicers: Dropdowns for date, city, country, and consumption type filters.

Dynamic Titles: Reflect active filters to enhance data interpretation.

🚀 How to Run

Clone the repository:

git clone <https://github.com/rishireddi/Energy-Consumption-Dashboard>

Open the Power BI .pbix file.

Refresh data connections if necessary.

Explore the dashboard by interacting with slicers and visuals.
