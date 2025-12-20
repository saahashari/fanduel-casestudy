# FanDuel Sportsbook Promotion Impact Case Study

Evaluate the incremental impact and ROI of a CRM Sportsbook promotion (run on **Jan 21, 2020**) using a **window-matched Difference-in-Differences (DiD)** design with **player-level** aggregation, **one-bonus-per-player** accounting, and **bootstrap confidence intervals** for decision-grade reporting.

---

## Business context

FanDuel ran a CRM Sportsbook promo on a selected target group of Sportsbook customers on **Jan 21, 2020** and wants to assess promo impact and ROI, including segment-level recommendations and supporting visualizations.

---

## Repository structure

```text
.
├── data/
│   └── FanDuel_CaseStudy_BusinessDataAnalysis.csv
├── notebooks/
│   ├── FanDuel_CaseStudy.ipynb
│   └── outputs/
│       └── crm_segment_recommendations.csv
├── Analyst_Business_Case_Questions_Instructions.docx
├── requirements.txt
├── .gitignore
└── README.md