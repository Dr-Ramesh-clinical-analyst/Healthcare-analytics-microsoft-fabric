# Healthcare Readmission Analytics | Microsoft Fabric & Power BI

## Project Overview

An end-to-end healthcare analytics project built using Microsoft Fabric and Power BI to analyze hospital readmissions and turn healthcare encounter data into actionable insights.

The project follows a medallion architecture—Bronze, Silver, and Gold—to organize data ingestion, transformation, validation, and analytics.

## Business Objectives

- Analyze hospital encounters and readmissions within 30 days.
- Explore the relationship between length of hospital stay and readmission metrics.
- Summarize readmission categories using interactive Power BI visuals.
- Validate analytical outputs before presenting them to stakeholders.

## Technology Stack

- **Microsoft Fabric** — Lakehouse and data engineering workflow
- **PySpark / Spark SQL** — Data transformation, where implemented
- **Power BI** — Interactive report and KPI visualization
- **GitHub** — Version control and project documentation

## Architecture

```text
Healthcare Source Dataset
          |
          v
   Bronze Layer
   Raw data ingestion
          |
          v
   Silver Layer
   Data cleaning and validation
          |
          v
    Gold Layer
   Analytics-ready tables
          |
          v
 Power BI Semantic Model
          |
          v
 Interactive Readmission Report
```

## Key Results

| Metric | Result |
|---|---:|
| Total hospital encounters | 101,766 |
| Readmissions within 30 days | 11,357 |
| Readmission rate within 30 days | 11.16% |

The readmission rate is calculated as readmissions within 30 days divided by total encounters.

## Dashboard Features

- KPI cards for total encounters and readmissions within 30 days.
- Column chart exploring readmission counts by length of hospital stay.
- Donut chart showing readmission status distribution.
- Hospital-stay and readmission-status slicers.
- Detail table containing length of stay, readmission metrics, and encounter counts.

**Note:** The current report uses separate Gold tables for some visuals, so not every slicer filters every visual. The report is an analytical demonstration, not a clinical decision-support system.

## Repository Structure

```text
Healthcare-analytics-microsoft-fabric/
├── data/
│   └── DATA_SOURCE.md
├── docs/
│   ├── architecture.md
│   └── data_dictionary.md
├── notebooks/
│   └── README.md
└── README.md
```

## Validation

The Gold-layer validation confirmed:

- 14 length-of-stay aggregation rows.
- 101,766 total encounters.
- 11,357 readmissions within 30 days.
- Validation status: passed.

## How to Explore This Project

1. Review `docs/architecture.md` for the project architecture.
2. Review `docs/data_dictionary.md` for documented fields and metrics.
3. Review `data/DATA_SOURCE.md` for source-data information.
4. Explore the notebooks documentation and available project artifacts.
5. Review the Power BI report screenshots when added to this repository.

The Microsoft Fabric workspace and report are hosted separately; access to those resources may require appropriate permissions.

## Future Enhancements

- Improve semantic-model relationships so relevant slicers filter all intended visuals.
- Add further demographic and clinical breakdowns where appropriate and supported by the data.
- Automate data-quality checks and document pipeline execution.
- Add dashboard screenshots and a project walkthrough.

## Disclaimer

This project is intended for educational and portfolio demonstration purposes. The analysis does not establish causation and must not be used as a substitute for clinical judgment.

---

**Author:** Dr-Ramesh-clinical-analyst  
**Repository:** [Healthcare-analytics-microsoft-fabric](https://github.com/Dr-Ramesh-clinical-analyst/Healthcare-analytics-microsoft-fabric)
# Microsoft Fabric Notebooks

## Purpose

This folder will contain notebooks used to ingest, clean, transform, and analyze the healthcare dataset using Microsoft Fabric and PySpark.

## Planned Notebooks

1. `01_bronze_ingestion.ipynb` — Load the source dataset into the Bronze layer.
2. `02_silver_transformation.ipynb` — Clean and validate the data.
3. `03_gold_analytics.ipynb` — Create analytics-ready tables and healthcare KPIs.

## Development Environment

The notebooks will be developed and executed in Microsoft Fabric. Notebook implementation and execution results will be added as the project progresses.

## Status

Notebook development is planned and has not yet been completed.
