# 🛒 Blinkit Grocery Sales and KPI Analysis

## 📝 Project Overview/Description

This project delivers a comprehensive business intelligence solution for analyzing Blinkit's grocery sales performance, customer satisfaction, and inventory distribution. The analysis leverages a combination of **SQL** for robust data cleaning and analytical querying, and **Power BI** for dynamic, interactive visualization.

The primary objective is to transform raw sales data into actionable business insights by:
1.  Establishing a reliable set of Key Performance Indicators (KPIs).
2.  Analyzing sales drivers and performance across various item categories and outlet types.
3.  Providing strategic recommendations to optimize sales and customer rating.

---

## 📈 Key Metrics and Insights

The analysis focuses on the following core metrics and dimensional views, as documented in the `Business_Requirement.pdf`:

### Core Key Performance Indicators (KPIs)

| Metric | Definition | Source File |
| :--- | :--- | :--- |
| **Total Sales** | The overall revenue generated from all sales. | `blinkit_kpi_queries.sql` |
| **Average Sales** | The average revenue generated per transaction. | `blinkit_kpi_queries.sql` |
| **Number of Items** | The total count of distinct items sold (or total orders/rows). | `blinkit_kpi_queries.sql` |
| **Average Rating** | The mean customer satisfaction rating for all items. | `blinkit_kpi_queries.sql` |

### Granular Analytical Dimensions

The project provides deep-dive analysis by segmenting sales and KPIs based on:
* **Item Characteristics:** Total Sales by Item Fat Content (e.g., 'Low Fat' vs 'Regular') and Item Type.
* **Outlet Demographics:** Performance segmented by Outlet Location Type (e.g., Tier 1, Tier 2), Outlet Size (Small, Medium, High), and Outlet Type (e.g., Supermarket Type1, Type2).
* **Time-based:** Total Sales by Outlet Establishment Year.

Key insights derived from this analysis are fully documented in the `Insights_Report.md`.

---

## 🛠️ How to Run and Utilize the Project

To replicate the analysis or interact with the dashboard, follow these steps:

### 1. Data Setup (SQL Database)
1.  Load the **`BlinkIT Grocery Data.csv`** file into your preferred SQL database (e.g., MySQL, PostgreSQL, or SQL Server).
2.  Execute the **`blinkit_cleaning.sql`** script to standardize inconsistent text fields (e.g., cleaning up `Item_Fat_Content` values) and ensure data quality.

### 2. Querying and Analysis
1.  Run the **`blinkit_kpi_queries.sql`** to calculate the main performance indicators.
2.  Run the **`blinkit_advanced_queries.sql`** to generate the segmented, dimensional data required for the deeper analysis and visualizations.
3.  Refer to **`Query_Documentation.pdf`** for detailed explanations of the logic used in each SQL query.

### 3. Visualization and Reporting
1.  Open the **`Blinkit_KPI_Dashboard.pbix`** file using Power BI Desktop.
2.  **Connect to Data Source:** Refresh the data connection, pointing it to your SQL database where the cleaned and queried tables reside.
3.  Review the **`Insights_Report.md`** for a written summary of the findings and strategic recommendations.

---

## 📂 Project Files

| File Name | Type | Description |
| :--- | :--- | :--- |
| `BlinkIT Grocery Data.csv` | Dataset | The **raw sales dataset** containing records, item details, outlet info, and ratings. |
| `blinkit_cleaning.sql` | SQL Script | Contains SQL commands to **clean and standardize** the raw data for consistent analysis. |
| `blinkit_kpi_queries.sql` | SQL Script | SQL queries to calculate **primary Key Performance Indicators (KPIs)**. |
| `blinkit_advanced_queries.sql` | SQL Script | SQL queries for **granular analysis** and segmentation by various dimensions. |
| `Business_Requirement.pdf` | Documentation | Outlines the **project scope, objectives**, and specific data requirements. |
| `Query_Documentation.pdf` | Documentation | Detailed **explanation and logic** behind all SQL scripts. |
| `Insights_Report.md` | Report | The final **written report** summarizing key findings and recommendations. |
| `Blinkit_KPI_Dashboard.pbix` | Power BI | The **interactive dashboard file** for visual data exploration. |

---

## 🤝 Contribution

Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to:

1.  **Fork** the repository.
2.  Create a new feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

Alternatively, open an issue with the tag "enhancement" or "bug."

---
