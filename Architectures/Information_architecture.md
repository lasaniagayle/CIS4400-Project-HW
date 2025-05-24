# Metro Bike Share Information Architecture

# Objective
The objective of this project is to analyze citywide bike share trip data to identify peak usage periods, understand spatial demand patterns, and guide strategic operational decisions such as bike redistribution, station placement, and service enhancement. The solution aims to support data-driven decision-making for both daily logistics and long-term transportation planning.

# Business Processes Supported / BI Solution Purpose
**Demand Forecasting:** Using past ridership data to predict future bike demand at different stations and times. This supports proactive planning for high-traffic areas.

**Operational Efficiency:** Identify station-level usage patterns and optimize the redistribution of bikes to prevent shortages or overcrowding.

**Service Planning:** Analyze spatial usage to support decisions on adding or relocating bike stations, ensuring underserved areas are prioritized.


**Analytics Required**
- Time-based analysis to identify usage peaks (e.g., morning commutes vs. weekend tourism).
- Geographic analysis to understand demand concentration by neighborhood/station.
- Membership analysis comparing casual vs. subscriber behavior.
- Dashboard visualizations for real-time and historical trip metrics.

**Decisions Affected:**
- Bike redistribution schedules and staffing.
- Station expansion planning and capacity adjustments.
- Pricing strategy and promotional targeting.
- Maintenance planning based on ride frequency and mileage.

# Stakeholders Granted Access

**Bike Share Operations Managers:** Monitor live usage, coordinate rebalancing, and schedule maintenance.


**Urban Planners/Transportation Departments:** Use spatial and temporal trends to improve infrastructure and connectivity.


**City Sustainability Offices:** Evaluate impact on emissions and equity in access.


**Marketing Teams:** Develop targeted campaigns based on user behavior trends.


**Data Analysts:** Monitor usage patterns, forecast demand, and report performance metrics.

# Data Overview

**Data Source:**
 Public trip data from the Metro Bike Share Data Portal, containing detailed logs of trips across the LA area.

**Integration Point:**
 CSV trip data is downloaded monthly, cleaned using ETL scripts (e.g., Python), then loaded into a cloud-hosted relational database for analysis.

**Consumption Pathway:**
 A business intelligence tool (Tableau) is used to visualize ridership patterns, generate usage reports, and support stakeholder decision-making.

**Technical Requirements**
- Integration with a scalable data warehouse (AWS Redshift )
- ETL pipeline using Python to clean and transform data
- Dash boarding and filtering capabilities through tools like Tableau or Power BI


