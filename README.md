
# AML Transaction Monitoring Dashboard

## Project Overview

This project analyzes a large synthetic transaction monitoring dataset using Power BI to explore transaction activity, identify patterns in transactions labelled as money laundering, and present findings through an interactive dashboard.

The dashboard is designed to support exploratory analysis by summarizing transaction activity, highlighting patterns across payment types and geographies, and providing transaction-level details for further investigation.

## Power BI Dashboard File

The Power BI dashboard file can be accessed here:

[Download the AML Transaction Monitoring Dashboard (.pbix)](https://drive.google.com/file/d/1n1dvmixN5WBg90px_J8102dnQtErcWeD/view?usp=sharing)

## Dataset

- **Dataset:** Synthetic Transaction Monitoring Dataset (SAML-D)
- **Source:** [Kaggle – Synthetic Transaction Monitoring Dataset (AML)](https://www.kaggle.com/datasets/berkanoztas/synthetic-transaction-monitoring-dataset-aml)
- **Nature of data:** Synthetic

The dataset contains approximately 9.5 million transactions. The labels are treated as provided in the dataset; they should not be interpreted as independently verified instances of financial crime.

## Tools and Technologies

- Microsoft Power BI
- Power Query
- DAX
- PostgreSQL

## Dashboard Pages

### 1. Executive Overview

Provides a high-level summary of transaction activity through key metrics and payment-type analysis, including:

- Total transaction value
- Total number of transactions
- Number and percentage of laundering-labelled transactions
- Average and maximum transaction amounts
- Transaction distribution across payment types

### 2. Patterns & Geography

Explores transaction patterns across locations, currencies, and time. This page includes:

- Sender and receiver bank locations
- Payment and received currency patterns
- Transaction activity over time
- Average transaction amounts by transaction label

### 3. Investigation & Suspicious Activity

Provides a more detailed view of laundering-labelled activity, including:

- Distribution by laundering type
- Transaction values across sender and receiver accounts
- Transaction-level details to support further examination

## Key Findings

The dashboard highlights the following patterns in the dataset:

- **9,873 transactions** are labelled as laundering, representing approximately **0.10%** of the total 9,504,852 transactions.
- The average transaction amount for laundering-labelled transactions was approximately **364.93% higher** than that of non-laundering-labelled transactions.
- Cross-border transactions recorded the highest number of laundering-labelled transactions among the payment types, with **2,628 transactions**.
- The UK was the most frequent receiver bank location among laundering-labelled transactions.
- UK Pounds was the most frequently recorded payment currency and received currency among laundering-labelled transactions.

These findings describe patterns in the dataset and do not, by themselves, establish that a transaction involved money laundering.

## Limitations

- The dataset is synthetic and may not reflect the full complexity of real-world financial transactions.
- Findings depend on the data and labels provided in the dataset.
- Transaction amounts are presented as represented in the source dataset; no currency conversion or normalization is assumed.

## Project Structure

```text
AML-Transaction-Monitoring/
├── README.md
├── AML_Transaction_Monitoring_Dashboard.pbix
└── Dashboard_Screenshots/
    ├── Page1_Executive_Overview.png
    ├── Page2_Patterns_Geography.png
    └── Page3_Investigation_Suspicious_Activity.png
```

## Disclaimer

This project is intended for learning, portfolio demonstration, and exploratory data analysis.
