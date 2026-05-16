# Workforce Retention Risk Analytics  
### A Portfolio-Enhanced HR Decision-Support Case Study

## 1. Project Overview

This project extends the original Google Advanced Data Analytics capstone into a portfolio-oriented workforce analytics case study.

The original capstone focuses on analyzing an HR dataset and building a predictive model to estimate whether an employee is likely to leave the company. The portfolio-enhanced version expands the project beyond model building by reframing it as a **workforce retention risk decision-support framework**.

Instead of only asking, “Can we predict employee attrition?”, this project asks:

> How can predictive analytics help HR stakeholders identify workforce risk patterns, understand potential drivers of employee turnover, and support more responsible retention strategies?

The project demonstrates how data analytics, machine learning, KPI design, stakeholder communication, and ethical considerations can be combined into a practical business decision-support workflow.

---

## 2. Business Problem

Employee turnover can create significant costs for organizations, including recruitment costs, onboarding costs, productivity loss, and knowledge loss.

In this case, the HR department wants to understand what factors may contribute to employee attrition and how data can support earlier intervention.

The key business questions are:

1. Which employee characteristics are associated with higher attrition risk?
2. How do workload, project burden, tenure, evaluation score, and promotion history relate to employee turnover?
3. Can a predictive model help identify employees or employee groups that may require HR attention?
4. How can model results be translated into practical and ethical workforce recommendations?

---

## 3. Project Goal

The goal of this project is to build a predictive and interpretive analytics workflow that supports HR decision-making.

The project aims to:

- Analyze employee attrition patterns through exploratory data analysis.
- Build classification models to predict whether an employee may leave.
- Identify important features related to attrition risk.
- Translate model results into HR-relevant risk indicators.
- Present the project as a portfolio-ready decision-support case.
- Highlight responsible and ethical use of predictive analytics in workforce management.

---

## 4. Dataset Description

The project uses an HR employee dataset from the Google Advanced Data Analytics capstone project. The dataset contains employee-level variables related to satisfaction, evaluation, workload, tenure, promotion history, department, salary, and attrition outcome.

The original dataset includes 14,999 rows and 10 columns.

Key variables include:

| Variable | Description |
|---|---|
| `satisfaction_level` | Employee-reported job satisfaction level |
| `last_evaluation` | Score of the employee’s last performance review |
| `number_project` | Number of projects assigned to the employee |
| `average_monthly_hours` | Average monthly working hours |
| `tenure` | Number of years the employee has worked at the company |
| `work_accident` | Whether the employee experienced a work accident |
| `left` | Whether the employee left the company |
| `promotion_last_5years` | Whether the employee was promoted in the last five years |
| `department` | Employee department |
| `salary` | Employee salary category |

The target variable is:

```text
left
```

where:

```text
0 = employee stayed
1 = employee left
```

---

## 5. Methodology: PACE Workflow

This project follows the PACE workflow:

```text
Plan → Analyze → Construct → Execute
```

### 5.1 Plan

The Plan stage defines the business problem, stakeholders, project goal, and analytical direction.

Key activities:

- Identify HR as the primary stakeholder.
- Define employee attrition as the prediction target.
- Reframe the project from a course-based prediction task into a business decision-support case.
- Consider potential ethical issues related to employee risk labeling and model misuse.

### 5.2 Analyze

The Analyze stage focuses on data understanding, cleaning, and exploratory data analysis.

Key activities:

- Inspect dataset structure and variable types.
- Rename columns for consistency.
- Check missing values.
- Identify duplicate records.
- Examine potential outliers.
- Explore relationships between attrition and workload, satisfaction, tenure, project count, salary, promotion, and department.

Important analytical themes:

- Employees with higher workload may face higher attrition risk.
- Project overload may be associated with employee turnover.
- Promotion history and tenure may provide useful retention-related signals.
- Satisfaction level is important but may raise data availability and leakage concerns in a real-world deployment setting.

### 5.3 Construct

The Construct stage develops classification models to predict employee attrition.

Models considered:

- Logistic Regression
- Decision Tree
- Random Forest

Key modeling steps:

- Encode categorical variables.
- Split data into training and testing sets.
- Train baseline and tree-based classification models.
- Evaluate performance using classification metrics.
- Compare model performance.
- Interpret feature importance.
- Consider data leakage and real-world model deployment limitations.

The enhanced portfolio version emphasizes not only predictive accuracy, but also interpretability and business usability.

### 5.4 Execute

The Execute stage translates analytical results into stakeholder-facing recommendations.

Key outputs:

- Model performance summary.
- Feature importance interpretation.
- Workforce risk insights.
- HR action recommendations.
- Ethical considerations.
- Dashboard planning for future Tableau visualization.

The goal is to help stakeholders understand what actions may reduce employee turnover risk, rather than simply identifying employees as likely to leave.

---

## 6. Portfolio Enhancement

This repository is not only a reproduction of the original capstone notebook. It adds a portfolio-oriented business analytics layer.

The enhanced version includes:

- Business problem reframing.
- HR stakeholder perspective.
- KPI-oriented interpretation.
- Workforce risk segmentation concept.
- Ethical analytics discussion.
- Tableau dashboard planning.
- GitHub Pages presentation.
- Public release boundary explanation.

The purpose is to demonstrate the ability to connect technical analytics with practical management decision-making.

---

## 7. Original GADA Capstone vs. Portfolio-Enhanced Version

| Dimension | Original GADA Capstone | Portfolio-Enhanced Version |
|---|---|---|
| Main Goal | Predict whether an employee will leave | Translate attrition prediction into HR decision support |
| Primary Audience | Course evaluator | Recruiters, HR stakeholders, consulting employers |
| Main Output | Notebook and project summary | GitHub Pages case study, README, KPI logic, dashboard plan |
| Analytical Focus | Classification model performance | Workforce risk, workload pressure, promotion gaps, retention strategy |
| Business Layer | Basic recommendation section | Stakeholder-oriented decision-support framing |
| KPI Design | Limited | Attrition rate, overwork rate, promotion gap, high-risk employee share |
| Ethical Layer | Basic ethical reflection | Employee labeling risk, model misuse, data leakage, fairness concerns |
| Portfolio Value | Demonstrates course completion | Demonstrates business analytics, communication, and decision-support ability |
| Professional Positioning | Data analytics student project | Applied analytics portfolio project |

---

## 8. Key Analytical Insights

The project identifies several potential attrition-related patterns:

1. Employees with very high monthly working hours appear more likely to leave.
2. Employees assigned to many projects may face higher workload pressure.
3. Employees with lower satisfaction levels are more likely to leave.
4. Promotion history may be relevant to retention risk.
5. Tenure may reveal important timing patterns in employee dissatisfaction or turnover.
6. Tree-based models can provide useful feature importance for stakeholder interpretation.

These insights should be interpreted carefully. The model is intended to support HR investigation and retention planning, not to automatically label or penalize employees.

---

## 9. Proposed HR KPI Framework

The portfolio-enhanced version introduces a KPI layer to make the project more useful for business stakeholders.

| KPI | Description | Business Purpose |
|---|---|---|
| Attrition Rate | Percentage of employees who left | Measures overall turnover level |
| Overwork Rate | Percentage of employees working above a defined monthly-hour threshold | Identifies workload pressure |
| Project Overload Rate | Percentage of employees assigned to many projects | Highlights project burden |
| Promotion Gap Rate | Percentage of employees not promoted in the last five years | Indicates potential advancement concern |
| High-Risk Employee Share | Percentage of employees predicted as high attrition risk | Supports HR prioritization |
| Average Monthly Hours | Average employee workload | Tracks workforce capacity pressure |

These KPIs can be used later in a Tableau dashboard to communicate findings more clearly.

---

## 10. Responsible Analytics and Ethical Considerations

Predictive analytics in HR must be handled carefully because model outputs can affect real people.

Important ethical considerations include:

| Ethical Issue | Risk | Mitigation |
|---|---|---|
| Employee labeling | Employees may be unfairly labeled as likely to quit | Use predictions for support, not punishment |
| Data leakage | Some variables may not be available or appropriate in real deployment | Test models with and without sensitive or leakage-prone variables |
| Managerial misuse | Results may be used to pressure or replace employees | Frame outputs as retention-support tools |
| Fairness concern | Department, salary, or promotion patterns may reflect structural inequities | Compare patterns across groups before acting |
| Transparency | Stakeholders may overtrust model results | Explain model limitations and feature importance clearly |

This project treats predictive modeling as a decision-support tool, not an automatic decision-making system.

---

## 11. Repository Structure

```text
workforce-retention-risk-portfolio/
├── index.html
├── README.md
├── assets/
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── main.js
├── data/
│   └── README.md
├── notebooks/
├── dashboard/
│   └── tableau_plan.md
├── docs/
│   └── project_summary.md
├── project-management/
│   └── stakeholder_map.md
└── references/
    └── source_log.md
```

---

## 12. Tools and Skills Demonstrated

| Category | Tools / Skills |
|---|---|
| Programming | Python |
| Data Manipulation | pandas, NumPy |
| Data Visualization | matplotlib, seaborn |
| Machine Learning | scikit-learn, decision tree, random forest, logistic regression |
| Model Evaluation | accuracy, precision, recall, F1-score, AUC |
| Business Analytics | KPI design, stakeholder framing, recommendation development |
| Portfolio Presentation | GitHub Pages, structured project documentation |
| Future Dashboard Design | Tableau planning |

---

## 13. Current Project Status

Current status:

```text
Repository published
GitHub Pages project page created
Portfolio enhancement layer added
README documentation in progress
Tableau dashboard phase planned
```

Planned next steps:

1. Finalize project documentation.
2. Add cleaned notebook or notebook summary.
3. Define Tableau dashboard KPI calculations.
4. Build Tableau dashboard.
5. Add Tableau Public link after publication.
6. Update the GitHub Pages project page with dashboard screenshots or embedded links.

---

## 14. Public Release Boundary

This repository is designed as a public-facing portfolio project.

The public version emphasizes:

- Project framing.
- Analytical workflow.
- Business interpretation.
- Model summary.
- Ethical considerations.
- Dashboard planning.

The public version may not include every experimental file, raw modeling artifact, or internal draft. This boundary helps keep the repository clear, professional, and employer-facing.

---

## 15. Project Positioning

This project demonstrates my ability to move beyond technical execution and connect analytics with business decision-making.

The main professional value of this project is not only that it builds a predictive model, but that it shows how a data professional can:

- Understand a stakeholder problem.
- Clean and analyze data.
- Build and evaluate models.
- Interpret results responsibly.
- Translate insights into practical recommendations.
- Communicate results through a portfolio-ready format.

This project supports my broader professional positioning at the intersection of transportation systems, data analytics, project management, and decision support.
