# Healthcare Analytics Project Architecture

## Objective

This project demonstrates how healthcare encounter data can be prepared and analyzed using Microsoft Fabric.

## Architecture

The project follows a Medallion Architecture:

**Source Dataset → Bronze → Silver → Gold → Power BI**

### 1. Bronze Layer — Raw Data

- Load the original diabetes hospital dataset.
- Preserve the source values.
- Inspect the schema and record count.
- Document the ingestion process.

### 2. Silver Layer — Cleaned Data

- Standardize column names and data types.
- Identify missing and duplicate records.
- Validate values and categories.
- Document data cleaning decisions.

### 3. Gold Layer — Analytics

- Create curated healthcare datasets.
- Calculate encounter and readmission metrics.
- Analyze hospital length of stay.
- Prepare tables for reporting.

### 4. Power BI — Reporting

The planned dashboard will include:
- Total hospital encounters.
- Readmission analysis.
- Length-of-stay patterns.
- Encounter characteristics.
- Data quality indicators.

## Technology Stack

- Microsoft Fabric Lakehouse
- PySpark and Python
- SQL
- Power BI
- GitHub

## Data Governance

The project will document data quality limitations and analytical assumptions. The historical dataset will be used for educational analysis, not clinical decision-making. The original dataset will not be uploaded to GitHub unless its terms permit redistribution.

## Project Status

Architecture documented; implementation is pending.
