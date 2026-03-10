# Credit Approval Fairness Audit

[![Analysis](https://img.shields.io/badge/analysis-responsible%20AI-blue)]()

---

**Full Governance Action Plan**

[View the Governance Action Plan](CreditModelGovernancePlan.pdf)

---


 **Full Investigation Report**  
[View the Credit Application Investigation](BankingCCApplicationsInvestigation-DinoFejzulovic.pdf)



The **Credit Approval Fairness Audit** is a data science and governance analysis project that investigates potential bias within an automated credit card approval model. Using a synthetic banking dataset, the project evaluates how geographic indicators such as postal codes may function as proxy variables and influence credit approval decisions.

The project demonstrates how **Responsible AI governance techniques** can be applied to automated financial decision systems. It includes both a **technical analysis notebook** and a **formal investigation report**, mirroring the type of fairness audits financial institutions conduct when reviewing automated credit decision models.

---

# Investigation Report

A full written investigation is included in this repository:

**Credit Application Investigation Report (PDF)**  
\`BankingCCApplicationsInvestigation-DinoFejzulovic.pdf\`

The report documents the governance review process, including:

- investigation scope and objectives  
- regulatory context within the Canadian banking system  
- dataset generation and model simulation methodology  
- fairness and bias evaluation metrics  
- geographic outcome analysis  
- governance conclusions and recommendations  

The report presents the analysis in the format of a **model governance investigation**, similar to internal reviews conducted by financial institutions when evaluating automated decision systems.

---

# Project Overview

The notebook performs a structured **Responsible AI governance review**, including fairness metrics, disparity analysis, and bias severity measurements similar to internal audits used by financial institutions to evaluate automated decision systems.

This project was conducted by **Dino Fejzulovic** as part of an independent investigation into **AI Governance and Responsible AI Ethics within the banking industry**, particularly the Canadian financial sector.

The dataset was loosely inspired by a publicly available Kaggle dataset:  
https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset

However, the dataset used in this analysis was **synthetically generated** to introduce controlled geographic bias patterns for the purpose of governance evaluation.

The analysis notebook was developed from scratch to demonstrate the application of Responsible AI governance principles in a credit approval context without replicating any existing codebase.

Since race is not collected in Canadian credit applications, the analysis focuses on **geographic indicators as potential proxies for socioeconomic status** and their impact on credit approval outcomes.

A **Postal Code Bias Severity Index** is introduced to quantify the magnitude of geographic bias within approval decisions, providing a novel monitoring metric that could be used during model governance reviews.

---

# Features

## Synthetic Banking Dataset Generation

- Generates thousands of simulated credit card applications.
- Includes financial attributes such as credit score, income, debt ratio, and payment history.
- Introduces geographic socioeconomic variation through postal codes.

## Automated Decision Simulation

- Computes approval outcomes using financial risk variables.
- Introduces controlled geographic penalties to simulate proxy bias.

## Fairness & Bias Analysis

- Approval rate analysis by postal code and regional income band.
- Disparate Impact Ratio calculations.
- Matched-profile fairness comparisons.

## Bias Severity Index

- Measures deviation between expected and actual approval rates.
- Identifies regions where approval outcomes diverge significantly from baseline expectations.

## Governance Visualizations

- Geographic bias heatmaps
- Expected vs actual approval comparisons
- Bias severity charts
- Credit profile vs decision outcome analysis

## Exportable Governance Outputs

- Analysis outputs exported as structured CSV reports for further governance review.

---

# Technology Stack

## Data Analysis

Python  
Pandas  
NumPy  

## Visualization

Plotly  

## Notebook Environment

Jupyter Notebook  

## Data Export

CSV reports for governance analysis

---


## Repository Structure

```
CreditApprovalFairnessAudit/
│
├── CreditApprovalFairnessAudit.ipynb
│   Main analysis notebook
│
├── BankingCCApplicationsInvestigation-DinoFejzulovic.pdf
│   Formal governance investigation report
│
├── generated_data/
│   Synthetic dataset outputs
│
├── governance_outputs/
│   Exported fairness metrics and governance reports
│
└── README.md
    Project overview and documentation
```

---

## Getting Started

### Prerequisites

- Python 3.10 or later
- pip
- Jupyter Notebook

### Clone the Repository

```bash
git clone https://github.com/DinoF15/CreditApprovalFairnessAudit.git
```

### Navigate to the Project

```bash
cd CreditApprovalFairnessAudit
```

### Install Dependencies

```bash
pip install pandas numpy plotly jupyter
```

### Run the Notebook

```bash
jupyter notebook
```

Open **CreditApprovalFairnessAudit.ipynb** and run the cells to reproduce the full governance analysis.

---

# Purpose of the Project

The purpose of this project is to demonstrate how **Responsible AI governance techniques** can be applied to automated financial decision systems.

Automated credit decision models can unintentionally learn patterns associated with geographic or socioeconomic characteristics. This investigation illustrates how financial institutions can detect such patterns using fairness metrics and governance monitoring tools.

The project is intended as a demonstration of **AI governance auditing methods**, not as a critique of any specific financial institution.

---

# Author

**Dino Fejzulovic**  
AI Governance & Responsible AI Research  
McMaster University 2026
