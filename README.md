Electric Vehicle Sales Analysis: SQL & Power BI Integration

This project demonstrates the seamless integration of **SQL** for data querying and **Power BI** for visualization to analyze electric vehicle (EV) sales trends in India. The workflow includes extracting insights like growth rates, penetration levels, and seasonal trends, then presenting them through interactive dashboards.

## Key Features
- **SQL Analysis**: In-depth queries to calculate metrics like EV adoption rates and trends.
- **Power BI Dashboards**: Dynamic visualizations for actionable insights.
- **Datasets**: Clean, structured data covering state-wise sales and manufacturer performance.

## Dataset Description

### 1. `electric_vehicle_sales_by_state.csv`
| Column Name               | Description                                                                                     | Data Type |
|---------------------------|-------------------------------------------------------------------------------------------------|-----------|
| `date`                    | Recording date (monthly). Format: `DD-MMM-YY`.                                                 | Date      |
| `state`                   | Indian state where sales were recorded.                                                        | String    |
| `vehicle_category`        | Vehicle type: `2-Wheeler` or `4-Wheeler`.                                                      | String    |
| `electric_vehicles_sold`  | Number of EVs sold in the state/category.                                                      | Integer   |
| `total_vehicles_sold`     | Total vehicles sold (EV + non-EV) in the state/category.                                       | Integer   |

### 2. `electric_vehicle_sales_by_makers.csv`
| Column Name               | Description                                                                                     | Data Type |
|---------------------------|-------------------------------------------------------------------------------------------------|-----------|
| `date`                    | Recording date (monthly). Format: `DD-MMM-YY`.                                                 | Date      |
| `vehicle_category`        | Vehicle type: `2-Wheeler` or `4-Wheeler`.                                                      | String    |
| `maker`                   | Manufacturer/brand of the EV.                                                                  | String    |
| `electric_vehicles_sold`  | Number of EVs sold by the maker in the category.                                               | Integer   |

### 3. `dim_date.csv` (Date Dimension Table)
| Column Name       | Description                                                                                     | Data Type |
|-------------------|-------------------------------------------------------------------------------------------------|-----------|
| `date`            | Date reference. Format: `DD-MMM-YY`.                                                           | Date      |
| `fiscal_year`     | Fiscal year (e.g., `2023`).                                                                    | Integer   |
| `quarter`         | Fiscal quarter (`Q1`, `Q2`, `Q3`, `Q4`).                                                       | String    |

## Tools Used
- **SQL**: Data extraction, transformation, and analysis (e.g., growth rate calculations).
- **Power BI**: Interactive dashboards with filters, maps, and trend visualizations.
- **Data Sources**: CSV files (provided in `/data` directory).
