# AI-Assisted Call Centre Optimisation & Service Analytics

Business analysis and service modernisation project for **Harbour Insurance Company**, focused on evaluating current call-centre performance and the feasibility of a **24/7 AI-assisted customer service model**.

This repository contains the Excel-based analytical workbook used for descriptive analytics, hypothesis testing, operational insights, and evidence to support management recommendations.

---

## Project Overview

Harbour Insurance Company operates four geographically distributed service centres across the UK:

- **Edinburgh** — Home Insurance
- **Liverpool** — Vehicle Insurance
- **Swansea** — Life Insurance
- **Luton** — Travel Insurance

Customers currently contact the company through four channels:

- **Call-Center**
- **Chatbot**
- **Email**
- **Web**

The business problem addressed in this project is whether Harbour's existing service model is still fit for purpose in 2025, and whether a redesigned **AI-assisted 24-hour service workflow** could improve service quality, reduce SLA breaches, and support future demand.

---

## Business Objective

The main objective of this project was to assess whether Harbour Insurance should modernise its customer support system by increasing automation through:

- AI chatbots
- prioritised webforms
- AI-assisted live call handling

The analysis aimed to answer four core questions:

1. Are current service channels meeting their **Service Level Agreements (SLAs)**?
2. Are **AI-supported channels** already performing well enough to justify expansion?
3. Do **channel type** and **geographic centre** materially affect operational performance?
4. Are **customer sentiment** and **enquiry reasons** distributed differently across centres?

---

## Dataset

The core dataset is contained in:

- `AI-Assisted Call Centre Optimisation & Service Analytics.xlsx`

### Workbook sheets

- **Descriptive Statistics** — pivot tables, summary views, charts, and operational findings
- **Hypothesis Tests** — z-tests, t-tests, and chi-squared tests
- **Customer Service** — underlying operational/customer service data used in the analysis

### Time period

- **May 2025 operational data**
- Weekly breakdowns from **week 0 to week 4**

### Variables analysed

The workbook analyses several operational and customer-experience variables, including:

- contact channel
- call centre location
- customer sentiment
- CSAT score
- time to answer
- call/contact duration
- issue reason
- customer counts
- week-based service patterns

---

## Analytical Approach

This project combines **descriptive analytics**, **inferential statistics**, and **simulation-based decision support**.

### 1) Descriptive analytics

Descriptive analysis was used to identify service patterns, bottlenecks, and customer-experience issues across channels and centres. This included:

- pivot tables
- summary statistics
- channel comparison charts
- centre-level performance comparisons
- reason/category frequency analysis
- sentiment distribution analysis

### 2) Hypothesis testing

Three main statistical techniques were used:

#### Z-test
Used to test whether the busiest channel was meeting the required SLA threshold.

#### T-test
Used to compare service performance between channels and compare Luton against other centres.

#### Chi-squared test
Used to test whether sentiment and enquiry reasons were independent of location.

### 3) Simulation modelling

The wider project also evaluated a **future-state AI-assisted operating model** using SIMUL8. Two system designs were compared:

- the **current service model**
- the **CEO's proposed 24/7 AI-assisted model**

The simulation objective was to assess whether the future design could handle **90,000 enquiries in a 4-week period**.

---

## Key Findings

### Operational findings

- **Negative sentiment dominates across all centres**, although the overall sentiment mix is broadly similar across locations.
- **Luton** appears to be the weakest-performing centre in terms of operational pressure and resolution time.
- **Edinburgh** performs best relative to the other centres.
- **Billing questions** are the most common reason for contact.
- **Call-Center** is the most used channel, followed by **Chatbot**.
- **Email** is the slowest and most inefficient channel in terms of resolution time.
- **Chatbot** is the strongest-performing channel against SLA expectations.
- Average **CSAT scores cluster around the mid-scale range**, indicating weak customer satisfaction.

### Channel performance summary

From the workbook's descriptive analysis:

| Channel | Avg. Time to Answer | Avg. Resolution / Contact Duration | Interpretation |
|---|---:|---:|---|
| Call-Center | 22 seconds | 2,228 seconds | Slightly above SLA for response time |
| Chatbot | 14 seconds | 509 seconds | Best-performing channel |
| Email | 10,057 seconds | 94,496 seconds | Major service bottleneck |
| Web | 13,300 seconds | 19,049 seconds | Slow engagement, moderate resolution delay |

---

## Statistical Test Results

### 1) Z-test: Is the busiest channel meeting SLA?

A z-test was used to determine whether **Call-Center time-to-answer** meets the **20-second SLA**.

**Result:** `p < 0.05`

**Interpretation:**
The null hypothesis was rejected. Call-centre response time is statistically **higher than the SLA threshold**, indicating an SLA breach.

### 2) Z-test: Is chatbot meeting SLA?

A one-sided z-test was used to assess whether **Chatbot time-to-answer** remains within the **20-second SLA**.

**Result:** `p > 0.05`

**Interpretation:**
The null hypothesis was not rejected. Chatbot performance is consistent with meeting the SLA and supports further investment in AI-enabled support.

### 3) T-test: Call vs Chatbot resolution time

A two-tailed t-test compared **Call-Center** and **Chatbot** contact duration.

**Result:** `p < 0.05`

**Interpretation:**
Channel type has a statistically significant effect on operational performance. Chatbots resolve issues much faster than live calls.

### 4) T-test: Is Luton worse than other centres?

A one-tailed t-test compared **Luton's mean resolution time** against the mean of the other centres.

**Result:** `p < 0.05`

**Interpretation:**
Luton's mean resolution time is significantly higher than the others, confirming it as the most problematic service centre in the current model.

### 5) Chi-squared test: Sentiment by centre

A chi-squared test assessed whether **sentiment category depends on call centre**.

**Result:** `p > 0.05`

**Interpretation:**
There is no statistically significant evidence that sentiment distribution differs by centre. Negative sentiment is widespread rather than isolated to only one location.

### 6) Chi-squared test: Issue type by centre

A chi-squared test assessed whether **enquiry reason depends on geography**.

**Result:** `p > 0.05`

**Interpretation:**
There is no statistically significant evidence that issue type differs across centres. The distribution of customer issues is broadly similar across locations.

---

## Management Insights

Based on the statistical and descriptive evidence, the most important business insights are:

- Harbour's **current SLA framework is outdated** relative to 2025 demand conditions.
- The business should **reduce dependency on human-only service delivery**.
- **Chatbot and webform channels should become the first-line support model**.
- **Billing and payment queries** are strong candidates for automation.
- The company should prioritise **service redesign in Luton** while standardising performance across all locations.
- AI investment appears more strategically valuable than simply increasing staff numbers.

---

## Recommended Future-State Model

This project supports a **tiered AI-assisted service model**:

### Stage 1 — 24/7 chatbot
First-line handling for routine and high-volume enquiries.

### Stage 2 — Prioritised webform
Escalation path for unresolved chatbot issues, with structured routing.

### Stage 3 — AI-assisted live call handling
Human support reserved for complex, high-value, or unresolved cases.

### Why this model?

Because the evidence suggests that:

- chatbots already outperform calls on SLA speed
- emails are inefficient and should not remain a primary resolution route
- many common enquiries are repetitive and automation-friendly
- human staff should focus on exceptions, escalation, and high-complexity cases

---

## Repository Structure

```text
.
├── AI-Assisted Call Centre Optimisation & Service Analytics.xlsx
├── README.md
└── images/                      
```

---

## Tools Used

- **Microsoft Excel** — pivot tables, charts, descriptive analytics, statistical calculations
- **SIMUL8** — simulation of current and future service models
- **Statistical testing** — z-test, t-test, chi-squared test
- **Business analysis techniques** — SLA review, service performance comparison, evidence-based recommendations

---

## How to Use This Repository

1. Download or clone the repository.
2. Open `AI-Assisted Call Centre Optimisation & Service Analytics.xlsx` in Microsoft Excel.
3. Review:
   - descriptive statistics
   - visual dashboards
   - hypothesis testing sheet
   - service insights and findings
4. Use the workbook to understand the evidence behind the proposed AI-assisted redesign.


---

## Limitations

- The analysis is based on a **single monthly review period (May 2025)**.
- Results should be interpreted as a **snapshot of performance**, not a long-term trend model.
- Some conclusions are operationally strong but would benefit from additional validation using:
  - multi-month data
  - cost-benefit analysis
  - customer preference segmentation
  - AI implementation risk assessment

---

## Future Work

Potential extensions for this project include:

- longitudinal sentiment analysis across multiple months
- cost-benefit analysis of AI adoption
- forecasting demand by issue type and channel
- testing staffing scenarios under different AI adoption rates
- building a Power BI or Python dashboard version of the Excel analysis

---

## Academic Context

This project was completed as part of the **MANP001 Assignment Case Study (Autumn 2025)**, focusing on service modernisation and AI-assisted call-centre design within my MSc in Data Science for Business.

> Note: Harbour Insurance Company is used here as part of an academic case study analysis.

---

## Author

**Muhammad Imran**  
Data Scientist 
GitHub: [@Imran3285](https://github.com/Imran3285)  
Email: m.imran88222@gmail.com

---

## License

This repository is for **educational and portfolio purposes** unless otherwise stated.
