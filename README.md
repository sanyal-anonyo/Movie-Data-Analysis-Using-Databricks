# Movie-Data-Engineering-Using-Databricks

## Overview

This project uses Databricks Medallion Architecture to build an automated movie data pipeline. Raw CSV data is ingested into the Bronze layer, cleaned and transformed into the Silver layer, and aggregated into Gold layer views for analytics. These views power Databricks dashboards for visualization, while a job pipeline automates the entire workflow for efficiency and scalability.


## PROBLEM STATEMENT

Organizations often struggle to efficiently process and analyze large volumes of raw data for actionable insights. In this case, a CSV file containing movie reviews and ratings from Netflix and Amazon Prime, including IMDb and Rotten Tomatoes scores, needs to be transformed into a structured, analytics-ready format. The challenge is to:
- Ingest raw data into a Bronze layer Delta table while preserving its integrity.
- Implement the Medallion Architecture to progressively refine data through Silver and Gold layers.
- Create interactive dashboards from Gold layer views for visualization and insights.
- Automate the entire workflow by designing a Databricks Job Pipeline, ensuring scalability, reliability, and repeatability.

### PROJECT DELIVERABLES

Following is a complete list of all project deliverables:
<table>
<tr><th>DELIVERABLE</th>	<th>DESCRIPTION</th></tr>
<tr><td>Bronze Layer Delta Table</td><td>	Ingest raw CSV file containing movie reviews and ratings into a Delta table, preserving original data.</td></tr>
<tr><td>Silver Layer Transformation	</td><td>Clean and standardize data from Bronze layer, ensuring quality and consistency for analytics.</td></tr>
<tr><td>Gold Layer Views</td><td>	Create curated and aggregated views from Silver layer for reporting and visualization.</td></tr>
<tr><td>Databricks Dashboard </td><td>	Develop interactive dashboards using Gold layer views to visualize insights on movie ratings.</td></tr>
<tr><td>Job Pipeline Automation	</td><td>Design and configure a Databricks Job Pipeline to automate ingestion, transformation, and dashboard updates.</td></tr>
</table>

![](Documentation/Architecture)


