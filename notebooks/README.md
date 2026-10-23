# Microsoft Fabric Notebooks

## Purpose

This folder documents the notebook workflow for the Healthcare Readmission Analytics project built with Microsoft Fabric and Power BI.

## Notebook Workflow

- **Bronze Ingestion:** Load the source healthcare dataset into the Bronze layer.
- **Silver Transformation:** Clean, transform, and validate the data.
- **Gold Analytics:** Create analytics-ready tables and readmission metrics.

## Development Environment

Microsoft Fabric is used for data engineering and analytics. PySpark and Spark SQL are used where implemented in the workflow.

## Current Status

The Fabric analytics workflow, Gold-layer aggregations, validation, and Power BI dashboard have been developed. Individual notebook files are not currently included in this GitHub folder. This README documents the intended processing stages.

## Related Documentation

- [Project Architecture](../docs/architecture.md)
- [Data Dictionary](../docs/data_dictionary.md)
- [Dataset Source](../data/DATA_SOURCE.md)
- [Main Project README](../README.md)
