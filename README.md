# ✈️ Emirates Airlines – Revenue & Route Profitability Analysis | Power BI

## Project Overview

This project focuses on analyzing airline revenue, route profitability, financial performance, passenger trends, and flight operations using an end-to-end data analytics workflow.

The objective was to transform raw airline data into meaningful business insights by combining data cleaning, Python-based data processing, SQL querying, database management, and interactive dashboard development.

The project follows a structured analytics pipeline, beginning with initial data preparation in Microsoft Excel and progressing through Python, PostgreSQL, and Microsoft Power BI.

## Project Objectives

- Analyze overall airline revenue, expenditure, and profitability.
- Identify the most profitable and loss-making flight routes.
- Evaluate financial performance across different routes and aircraft types.
- Understand passenger traffic, demand patterns, and aircraft utilization.
- Examine individual cost components and their contribution to total expenditure.
- Analyze monthly and seasonal business performance.
- Develop an interactive Power BI dashboard to present business insights effectively.

## Technology Stack

| Technology | Application |
|---|---|
| Microsoft Excel | Initial data cleaning and preparation |
| Python | Data inspection and transformation |
| Pandas & NumPy | Data manipulation and validation |
| Jupyter Notebook | Executing and documenting Python workflows |
| PostgreSQL | Relational database management |
| SQL | Business analysis and querying |
| Microsoft Power BI | Interactive dashboard development |
| DAX | Calculated measures and KPIs |

## End-to-End Project Workflow

### 1. Initial Data Cleaning – Microsoft Excel

The initial dataset was processed using Microsoft Excel to prepare it for further analysis.

Key activities included:
- Reviewing the dataset structure and identifying inconsistencies.
- Performing initial data cleaning and preparation.
- Standardizing data where required.
- Preparing the dataset for Python-based processing.

### 2. Data Cleaning & Validation – Python, Pandas and Jupyter Notebook

The dataset was imported into Jupyter Notebook using Pandas for further inspection and transformation.

Key activities included:

- Importing the dataset using Pandas.
- Standardizing column names by converting them to lowercase and replacing spaces with underscores.
- Inspecting missing values across columns.
- Checking for duplicate records.
- Identifying negative values in numerical columns.
- Validating load factor values to identify values outside the expected 0–1 range.
- Checking whether passenger counts exceeded aircraft capacity.

NumPy and Pandas were used as part of the data-processing workflow.

The cleaned dataset was subsequently prepared for database integration.

### 3. Database Integration – PostgreSQL

After data preparation, the cleaned dataset was imported into PostgreSQL using SQLAlchemy.

The database was named:

`emirates_airlines_db`

The primary table was:

`emirates_airlines_route_profitability`

Python's `to_sql()` functionality was used to load the processed Pandas DataFrame into PostgreSQL.

This established a structured database environment for performing SQL-based analysis and connecting the data to Power BI.

### 4. SQL Business Analysis – PostgreSQL

SQL was used to explore the dataset and answer business-oriented analytical questions.

A total of 24 SQL business queries were developed, covering the following areas:

**A. Financial Performance Analysis**
- Total flights, passengers, revenue, costs, and profit.
- Average load factor and profit margin.
- Business performance across different seasons.
- Revenue and profit by demand category.
- Monthly revenue and profitability trends.
- Highest and lowest profit-generating months.
- Revenue contribution by source.
- Cost components contributing to total expenditure.

**B. Route Performance Analysis**
- Profitability across route categories.
- Top 10 most profitable routes.
- Top 10 revenue-generating routes.
- Routes operating at a financial loss.
- Routes with the highest profit margins.
- Origin and destination combinations with the highest load factor.

**C. Passenger & Demand Analysis**
- Monthly passenger traffic trends.
- Top 10 routes by passenger traffic.
- Passenger demand across different seasons.
- Passenger traffic by demand category.
- Load factor and profit margin across demand levels.

**D. Aircraft & Operational Analysis**
- Passenger and capacity analysis by aircraft type.
- Average profit by aircraft type.
- Average flight duration by aircraft type.
- Flight duration and passenger utilization by route.

The SQL queries were executed through Python using SQLAlchemy and Pandas, and their results were collected for further analysis and reporting.

### 5. Interactive Dashboard Development – Microsoft Power BI

The processed data was connected directly from PostgreSQL to Microsoft Power BI.

The dashboard was developed using DAX measures, KPI cards, charts, slicers, and interactive visualizations.

The report is organized into five analytical pages:

#### Page 1 – Airline Business Overview

Provides a high-level overview of the airline's overall business performance.

Key KPIs:
- Total Revenue
- Total Cost
- Total Profit
- Total Flights
- Total Passengers
- Profit Margin

#### Page 2 – Route Performance Analysis

Focuses on evaluating the financial performance of individual flight routes.

Key KPIs:
- Total Routes
- Profitable Routes
- Loss-Making Routes
- Average Profit Margin
- Average Profit per Route
- Total Destinations

#### Page 3 – Financial Performance Analysis

Provides insights into the airline's financial performance through revenue, expenditure, and profitability analysis.

Key KPIs:
- Total Revenue
- Total Cost
- Total Profit
- Profit Margin
- Revenue per Flight
- Cost per Flight

#### Page 4 – Passenger Trends & Insights

Analyzes passenger traffic, demand, and aircraft capacity utilization.

Key KPIs:
- Total Passengers
- Average Passengers per Flight
- Average Load Factor
- Total Capacity
- Available Seats
- Passenger Revenue

#### Page 5 – Flight Operations & Fleet Performance

Focuses on aircraft utilization and operational performance.

Key KPIs:
- Total Flights
- Total Flight Hours
- Average Flight Duration
- Average Aircraft Capacity
- Average Load Factor
- Total Passengers

### 6. Data Modeling & DAX

DAX measures were created to calculate important business metrics and KPIs.

Additional data modeling was performed to support analytical requirements, including date-based analysis and cost component breakdowns.

Interactive slicers and filters were incorporated to allow users to explore the data across different dimensions.

## Dataset Information

The project uses an airline route profitability dataset covering flight-level operational and financial information.

| Attribute | Details |
|---|---|
| Dataset | Emirates Airlines Route Profitability |
| Records | 7,974 |
| Columns | 33 |
| Data Period | January – December 2024 |
| Origin | Dubai (DXB) |
| Destinations | 30 |
| Aircraft Types | 6 |

The dataset includes flight dates, flight numbers, routes, aircraft types, passenger counts, aircraft capacity, load factor, revenue streams, individual cost components, total revenue, total cost, profit, and profit margin.

## Key Learning Outcomes

Through this project, I gained practical experience in:

- Performing data cleaning and validation using Excel and Python.
- Working with Pandas and NumPy for data manipulation.
- Connecting Python applications to PostgreSQL using SQLAlchemy.
- Writing SQL queries to solve business-oriented analytical questions.
- Understanding relational database integration with Power BI.
- Creating DAX measures and business KPIs.
- Developing interactive dashboards and presenting analytical findings.
- Following an end-to-end data analytics workflow.


## Project Files

- **Jupyter Notebook:** Contains the Python-based data inspection, validation, PostgreSQL integration, and SQL query execution workflow.
- **SQL Script:** Contains the PostgreSQL business analysis queries.
- **Power BI File:** Contains the interactive dashboard and associated data model.
- **Cleaned Dataset:** Contains the processed airline dataset used in the project.

## Disclaimer

*This project has been developed solely for educational, learning, and portfolio demonstration purposes. It is an independent project and has no affiliation, association, sponsorship, or endorsement from Emirates Airlines. The company name and trademarks belong to their respective owners. All analyses and insights are based on the dataset used in this project and do not represent the company's official financial or operational performance.*

## Conclusion

This project provided an opportunity to apply data analytics concepts to an airline business scenario by integrating multiple technologies into a single workflow.

From initial data preparation and validation to SQL-based business analysis and interactive Power BI reporting, the project demonstrates the practical application of data analytics tools in transforming raw data into meaningful business insights.

## 👨‍💻 Author

**Ved Patil** | [LinkedIn](https://linkedin.com/in/vedpatil3076/)

Aspiring Data Analyst | Business Intelligence Enthusiast

**Technologies:** SQL | PostgreSQL | Power BI | DAX
