# Healthcare Dataset Data Dictionary

## Overview

This document describes selected columns from the Diabetes 130-US Hospitals for Years 1999–2008 dataset.

## Selected Fields

| Column | Description |
|---|---|
| `encounter_id` | Identifier for a hospital encounter |
| `patient_nbr` | Patient identifier; multiple encounters may belong to one patient |
| `race` | Recorded race category |
| `gender` | Recorded gender |
| `age` | Patient age range |
| `admission_type_id` | Coded hospital admission type |
| `discharge_disposition_id` | Coded discharge disposition |
| `admission_source_id` | Coded admission source |
| `time_in_hospital` | Number of days spent in hospital |
| `num_lab_procedures` | Number of laboratory procedures |
| `num_procedures` | Number of other procedures |
| `num_medications` | Number of medications recorded |
| `number_outpatient` | Outpatient visits in the preceding year |
| `number_emergency` | Emergency visits in the preceding year |
| `number_inpatient` | Inpatient visits in the preceding year |
| `diag_1` | Primary diagnosis code |
| `diag_2` | Secondary diagnosis code |
| `diag_3` | Additional diagnosis code |
| `readmitted` | Recorded readmission category |

## Data Quality Considerations

- Some columns contain missing or unknown values.
- Several fields use coded values that require interpretation using the dataset documentation.
- Multiple encounters may belong to the same patient.
- Readmission categories must be interpreted according to the original dataset definitions.

## Source

[UCI Machine Learning Repository — Diabetes 130-US Hospitals](https://archive.ics.uci.edu/dataset/296/diabetes+130-us-hospitals+for+years+1999-2008)

## Project Status

Initial data dictionary drafted. Definitions will be validated during data ingestion and analysis.
