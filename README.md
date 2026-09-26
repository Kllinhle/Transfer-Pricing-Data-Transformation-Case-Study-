# Transfer Pricing Data Transformation Case Study

## Overview

A data transformation and compliance analysis project focused on using transaction-level data to identify **transfer pricing compliance risks, data-quality issues, and opportunities for process automation**.

The project demonstrates the process from **raw transaction data → data cleaning → margin calculation → compliance assessment → risk analysis → automation recommendations**.

## Objective

The objective was to transform raw transaction data into actionable insights by:

* Standardising and cleaning transaction data
* Converting transaction values into EUR
* Calculating transaction margins
* Assessing transactions against transfer pricing benchmarks
* Identifying high-risk countries and transaction types
* Identifying data-quality and process risks
* Proposing opportunities for automation and dashboarding

## Analysis Approach

### 1. Data Preparation

* Removed 5 fully identical duplicate records
* Standardised entity names, countries, and transaction types
* Standardised date formats
* Converted transaction amounts into EUR
* Flagged missing data rather than removing incomplete records
* Calculated transaction margin where sufficient data was available

**Margin formula:**

`Margin % = (Amount - Cost Base) / Cost Base`

### 2. Compliance Assessment

Transactions were assessed against predefined arm's-length benchmark ranges:

| Transaction Type | Benchmark |
| ---------------- | --------: |
| Goods            |     3%–8% |
| Services         |    5%–10% |
| Royalties        |    8%–15% |

Each transaction was classified as:

* Compliant
* Non-compliant
* Unknown

## Key Findings

* **77%** of transactions were classified as non-compliant
* **13%** had an unknown compliance status
* **Goods** had the highest non-compliance rate at **32.2%**
* **Royalties** followed at **26.44%**
* France, Germany, and Poland showed notable country-level compliance risks
* Missing data and incomplete information created limitations for reliable risk monitoring

## Risk & Process Improvement

The analysis identified three main risk areas:

1. **High non-compliance exposure**
2. **Data-quality and missing-data issues**
3. **Concentration of compliance issues in specific transaction types**

Recommended improvements include:

* Standardised global TP templates
* Automated data-validation rules
* Automated TP deviation flagging
* Clear ownership and escalation procedures
* Periodic compliance monitoring and KPIs

## Automation Opportunities

The analysis also explores how the process could be further automated through:

**Power BI**

* Compliance dashboards
* Country and transaction-type risk monitoring
* High-risk transaction matrices
* Automated reporting

**AI**

* Identifying inconsistencies in TP documentation
* Detecting unusual transaction patterns
* Prioritising high-risk cases
* Supporting annual documentation updates

## Tools & Skills

**Excel · PivotTables · Data Cleaning · Data Transformation · Data Analysis · Transfer Pricing · Risk Analysis · Process Improvement · Automation**

## Project Files

* `TP_case_dataset_cleaned.xlsx` — cleaned and transformed transaction dataset
* `TP_case_study.pdf` — full case study and analysis

