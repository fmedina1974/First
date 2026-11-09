# QGSO-style R practice simulation

## Scenario
You are a Senior Statistician/Analyst in a fictional Crime Statistics team.
You receive administrative extracts from police, courts and corrections.
Your task is to quality-assure the data, produce annual statistical outputs,
and prepare a simple forecasting product for internal stakeholders.

The datasets are synthetic. They are designed to resemble the types of
administrative-data issues a statistical production team may encounter.

## Files
1. police_incidents.csv
2. court_matters.csv
3. corrections_admissions.csv
4. population_monthly.csv

## Stage 1 — Import and initial quality checks
Using R:
- Import all four files.
- Inspect structure, types, missing values and duplicate identifiers.
- Check date ranges.
- Identify inconsistent categorical values.
- Identify impossible or suspicious values.
- Produce a short quality-issues table.

## Stage 2 — Clean and standardise
Create cleaned versions of the datasets:
- Standardise region and offence-group labels.
- Resolve exact duplicate records.
- Flag invalid ages rather than silently deleting them.
- Flag court matters where finalisation precedes lodgement.
- Flag corrections records where expected release precedes admission.
- Keep an audit trail of the changes you make.

## Stage 3 — Statistical production
Produce:
- Annual police incident counts by offence group, 2019–2025.
- Annual police incident rate per 100,000 population by region.
- Annual court lodgements and finalisations.
- Median days from court lodgement to finalisation by year.
- Annual corrections admissions by custody type.
- A one-page summary table for 2025.

## Stage 4 — Join and interpret
- Link court matters to police incidents using incident_id.
- Calculate the proportion of court matters linked to each offence group.
- Identify any records that fail to link and explain how you would investigate them.
- Write 3–5 sentences explaining one notable trend without overstating causation.

## Stage 5 — Forecasting
Build a monthly time series of court lodgements.
- Plot the series.
- Inspect trend and seasonality.
- Fit a reasonable forecasting model in R.
- Produce a 12-month forecast with prediction intervals.
- Compare at least two candidate models or specifications.
- Explain how you would validate and monitor the forecast in production.

## Stage 6 — AO7-style judgement
Prepare a short note (max 250 words) to a Team Leader covering:
- the main data-quality risks;
- one important statistical trend;
- the forecast result;
- one limitation;
- one recommendation for improving the production process.

## What this exercise is testing
This is not a test of crime-law knowledge. It is designed to test the R/data
skills most relevant to the role:
- data import and transformation;
- joins and administrative-data management;
- validation and quality assurance;
- reproducible code;
- statistical production;
- time-series analysis and forecasting;
- interpretation and communication.

Do not try to complete everything at once. Start with Stage 1.
