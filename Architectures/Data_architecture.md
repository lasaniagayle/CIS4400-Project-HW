# Metro Bike Share Data Architecture

# Overview
The data architecture for this project outlines how Metro Bike Share data will be sourced, processed, stored, and consumed. It ensures that the information architecture’s analytical needs are met by providing structured data pipelines and storage, maintaining data quality, and enabling effective reporting.

# Key Components

**Source Systems**

Metro Bike Share Open Data Portal:
 - Raw trip data in CSV format, published monthly, includes trip ID, duration, start/end station, timestamps, pass type, and bike ID.

**Data Integration & ETL Process:**

- Tools: Python scripts and cloud-based tools (Azure)

**ETL Workflow:**

- Extract CSV files from the public portal.

- Cleanse and normalize data (e.g., standardize timestamps, handle missing values).

- Transform fields (e.g., calculate trip duration in minutes, extract date/time dimensions).

- Load into a centralized cloud database (AWS Redshift).


# Master Data Management (MDM)

**Define and standardize reference data:**
- Station names and IDs
- Pass type categories (Monthly, Flex, Walk-up)
- Ensure consistency across monthly data files and time series.


**Data Quality** 

**Implement validation checks:**
- Remove incomplete or duplicate trips.
- Verify timestamp formats and station matching.
- Identify and correct outliers in trip duration.

# Enterprise Data Warehouse (EDW)

**Storage Format:** 
 - Star schema with a fact table (Trips) and dimension tables (Date, Station, User Type)

**Scalability:**
 - Cloud-native architecture for flexible storage and querying large amount of records.

# Information Consumption (BI Tools)
 
 **Tableau dashboards used for:**

- Visualizing bike trip patterns
- Filtering data by time, station, and user type
- Generating reports for planning and operations
- Data Analysts and Stakeholders: Access reports through secure dashboards with role-based permissions.

# Benefits
- Supports operational decision-making through reliable and timely insights.
- Enables data governance by applying master data and quality standards.
- Scales to accommodate new trip data over time.
- Facilitates secure access and intuitive reporting for non-technical stakeholders.
