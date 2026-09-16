

# AI-Powered Paper Purchase Optimization Decision Support System
<img width="922" height="494" alt="Screenshot 2026-07-24 123115" src="https://github.com/user-attachments/assets/fc66a75c-35a9-4e90-8426-115755aa4b66" />



> Balancing Prediction and Constraint: An Optimization-Based Decision Support System for Job-to-Order Print Manufacturing

An end-to-end Machine Learning + Optimization project that helps print manufacturing companies make smarter paper purchasing decisions under demand uncertainty, budget constraints, and storage limitations.

MSc Data Science Final Project – University of Europe for Applied Sciences

Authors: Renato Mateo Silva • Sandra Raj Pattuvakkaran • Okah Ahone Ebwekoh • Sudarsh Mekkampurath Sajeev

## Project Overview

Job-to-order print manufacturers often struggle with purchasing the right amount of paper because quoted material estimates frequently differ from actual consumption.

This project develops an Optimization-Based Decision Support System (DSS) that combines a Linear Regression model with a Newsvendor Optimization Model to generate data-driven purchasing recommendations while considering real business constraints such as budget and storage capacity.

Final Report DSS.pdf

## Business Problem

Production managers face two costly risks:

* Under-purchasing: Production delays and missed delivery commitments.

* Over-purchasing: Excess inventory, tied-up capital, and storage costs.

The objective is to minimize total expected purchasing costs while accounting for uncertainty in actual paper consumption.

Final Report DSS.pdf

## Solution Architecture

![Predicting Demand in Supply Chain Management: A Decision Support System Using Graph Convolutional Networks](https://images.openai.com/static-rsc-4/z87FFMsJC6EkxeWBvnM4Wsk1FZRmRX7rkMGQUaD1NqKIeusI9wSgjTWpcim5ASAYtMNbV9pYzLdxqbKgj2K8RBRqDaik1fAu9ztKIchiQyCX7rvZMtH5khXAwkfCY_QSXG3yaH1niwJyc-gNFFdfs6WwGRz4rZYAJJZBUrAD5pU?purpose=inline)

The system follows a structured workflow:

1. Enter current production orders.

2. Predict paper requirements using historical production data.

3. Estimate demand uncertainty.

4. Calculate the available monthly purchasing budget.

5. Optimize purchase quantity using the Newsvendor Model.

6. Generate a final purchasing recommendation.

   Final Report DSS.pdf

   Final Report DSS.pdf

## Methodology

### Machine Learning

A Linear Regression model predicts expected paper cost using:

* Business Line

* Job Type

* Order Quantity

### Optimization

A Newsvendor Optimization Model converts predicted demand into an optimal purchase recommendation while balancing:

* Holding Cost

* Stockout Cost

* Budget Constraints

* Storage Capacity

Rather than only forecasting demand, the system produces an actionable business decision.

Final Report DSS.pdf

Final Report DSS.pdf

## Tech Stack

|
Category

|

Tools

|
| --- | --- |
|

Programming

|

Python

|
|

Data Processing

|

Pandas

|
|

Machine Learning

|

Scikit-learn

|
|

Optimization

|

SciPy

|
|

Decision Support

|

Newsvendor Model

|
|

Analytics

|

Statistical Modeling

|

## Dataset

The project uses real manufacturing records.

Primary datasets

* `master_cotizaciones.csv` (Quotation Data)

* `master_ordenes_ejecutivo.csv` (Completed Production Orders)

Historical quotations were matched with completed production orders to train and validate the prediction model.

Final Report DSS.pdf

## Key Features

* Machine Learning-based paper demand prediction

* Demand uncertainty estimation

* Dynamic monthly budget calculation

* Newsvendor purchase optimization

* Scenario analysis under different business policies

* Transparent and explainable recommendations

## Results

The system was validated using 55 historical production orders across multiple purchasing scenarios.

Final Report DSS.pdf

|
Metric

|

Result

|
| --- | --- |
|

Validation Batch

|

55 Orders

|
|

Baseline Gap

|

11% below actual material need

|
|

Best Scenario

|

11.3% above actual need

|
|

Primary Constraint

|

Budget Policy

|

### Key Insight

The most important finding was that the organization's budget policy—not the prediction model—was the dominant factor limiting purchasing decisions.

Even when operational risk assumptions changed, the final recommendation remained constrained by the available budget, demonstrating how optimization can reveal hidden business bottlenecks.

Final Report DSS.pdf

## Scenario Analysis

Four operational scenarios were evaluated:

|
Scenario

|

Purpose

|
| --- | --- |
|

Base Case

|

Current operating conditions

|
|

Worst Case

|

Higher production risk

|
|

Finance Conservative

|

Lower spending tolerance

|
|

Production Conservative

|

Higher safety stock

|

The production-focused scenario was the only one that fully covered actual material requirements.

Final Report DSS.pdf

## Business Impact

This Decision Support System replaces experience-based purchasing decisions with a structured, data-driven, and risk-aware recommendation by:

* Improving inventory decision-making

* Quantifying the impact of business constraints

* Supporting explainable purchasing recommendations

* Enabling scenario-based decision analysis

  Final Report DSS.pdf

## Future Improvements

Planned enhancements include:

* Forecasting incoming production orders

* Adding richer production features (page count, paper specifications)

* Validating across multiple production periods

* Improving prediction accuracy while maintaining model transparency

* Integrating prediction and budgeting into a unified workflow

  Final Report DSS.pdf

## Repository Structure

```
AI-Paper-Purchase-DSS/
│
├── data/
│   ├── master_cotizaciones.csv
│   └── master_ordenes_ejecutivo.csv
│
├── notebooks/
├── models/
├── optimization/
├── report/
│   └── Final_Report.pdf
│
└── README.md
```

## Skills Demonstrated

* Machine Learning

* Linear Regression

* Decision Support Systems

* Operations Research

* Inventory Optimization

* Newsvendor Model

* Python

* Pandas

* Scikit-learn

* SciPy

* Business Analytics

* Explainable AI

## Author

Sandra Raj Pattuvakkaran

MSc Data Science | Python | Machine Learning | Business Analytics | Decision Support Systems | Operations Research


