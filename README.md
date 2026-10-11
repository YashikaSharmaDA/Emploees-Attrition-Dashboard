# Employee Attrition Analytics | Microsoft Fabric + Power BI

> Why are employees leaving? An end-to-end analytics solution built in Microsoft Fabric.


## Business problem
Attrition is 16.1% (237 of 1,470 employees). HR needs to know where, who and why.

## Key insights
- Sales Representatives show 39.8% attrition, the highest of any role
- Employees earning under 3k leave at 28.6% vs 10.4% above 10k
- Overtime nearly triples attrition (30.5% vs 10.4%)
- Single employees and the 18–25 age group are most at risk

## Architecture
(mermaid diagram)

## Tech stack
Microsoft Fabric (Workspace, Dataflow Gen2, Lakehouse, Semantic Model),
Power BI, DAX, Power Query (M), OneLake data access roles (CLS)

## Data
Source, license, row count, data dictionary → see /data

## Data preparation
Cleaning steps, derived columns (Salary band, Age group), data types

## Data model & DAX
Key measures: Attrition Rate, Headcount, Attrition Left, Avg Tenure of Leavers

## Dashboard pages
Overview: KPIs, department and role breakdown, decomposition tree
Detailed Summary: performance, travel, overtime, marital status, age and gender

## Security
CLS on HR_empl via lakehouse role (sensitive columns hidden from readers)

## Recommendations
1. Review compensation for under-3k roles
2. Cap overtime in Sales
3. Early-career retention program
