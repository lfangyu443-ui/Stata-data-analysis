# Stata-data-analysis
This repository contains the Stata scripts and associated datasets used for data analysis
# Analysis of Categorical Data using STATA

**Module:** SPH5006 Epidemiology and Statistical Methods, NUS Saw Swee Hock School of Public Health  
**Date:** October 2025

---

## Overview

Practical and written assignment applying categorical data analysis techniques in STATA, 
covering odds ratio, risk ratio, chi-square trend test, and McNemar's test across 
different epidemiological study designs.

---

## Analyses Performed

| Analysis | STATA Command | Dataset | Study Design |
|----------|--------------|---------|--------------|
| Odds ratio + 95% CI | `cci`, Woolf method | myopia.dta | Case-control |
| Risk ratio + 95% CI | `csi` | myopia.dta | Cohort |
| Chi-square + Fisher's exact | `tabi` | toxaemia.dta | Cross-sectional |
| Chi-square trend test | `tabodds [fweight=freq]` | toxaemia.dta | Ordered categories |
| Odds ratio by category | `tabodds, or` | toxaemia.dta | Case-control |

---

## Key Results

**Myopia dataset** — association between near work and myopia:
- Odds ratio: 2.80 (95% CI: 1.44 – 5.45, p = 0.002)
- Risk ratio: 1.96 (95% CI: 1.32 – 2.91, p = 0.002)

**Toxaemia dataset** — association between diet quality and pre-eclamptic toxaemia:
- Significant linear trend: odds of toxaemia decrease as diet quality improves (χ²(1) = 14.80, p < 0.001)
- Compared to very poor diet, good diet OR = 0.10 (95% CI: 0.02 – 0.44, p < 0.001)

---

## Skills Demonstrated

- Selecting appropriate effect measures by study design (OR vs RR vs PR)
- Applying frequency weights for grouped data (`fweight`)
- Chi-square trend test for ordered categorical exposures
- Interpreting Woolf confidence intervals
- Recognising the importance of loading frequency weights before `tabodds`

---

## Repository Contents
```
02_categorical-data-stata/
├── README.md
├── Analysis of Categorical Data.log     ← STATA output
├── Analysis_of_Categorical_Data.docx    ← written assignment
└── data/
    ├── myopia.dta
    └── toxaemia.dta
```

---

## Note

This work was completed as part of SPH5006 at NUS Saw Swee Hock School of Public Health.
