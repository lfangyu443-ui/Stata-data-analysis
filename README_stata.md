# 📊 Stata Data Analysis — Epidemiological & Health Data

![Stata](https://img.shields.io/badge/Stata-1A5276?style=flat)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat)
![Domain](https://img.shields.io/badge/Domain-Public%20Health-teal?style=flat)

Stata scripts and written assignments from **SPH5006 Epidemiology and Statistical Methods** at NUS Saw Swee Hock School of Public Health. Each analysis is documented with interpretation of results, not just code.

---

## 📁 Projects

### 1. Analysis of Categorical Data
**Date:** October 2025 | **Module:** SPH5006, NUS

Practical assignment applying categorical data analysis techniques to real epidemiological datasets.

| Analysis | Command | Dataset | Study Design |
|---|---|---|---|
| Odds ratio + 95% CI | `cci`, Woolf method | myopia.dta | Case-control |
| Risk ratio + 95% CI | `csi` | myopia.dta | Cohort |
| Chi-square + Fisher's exact | `tabi` | toxaemia.dta | Cross-sectional |
| Chi-square trend test | `tabodds [fweight=freq]` | toxaemia.dta | Ordered categories |
| OR by category | `tabodds, or` | toxaemia.dta | Case-control |

**Key findings:**
- Near work and myopia: OR = 2.80 (95% CI: 1.44–5.45, p = 0.002); RR = 1.96 (95% CI: 1.32–2.91)
- Diet quality and pre-eclamptic toxaemia: significant linear trend (χ²(1) = 14.80, p < 0.001); good diet vs. very poor diet OR = 0.10 (95% CI: 0.02–0.44)

**Skills demonstrated:**
- Selecting effect measures by study design (OR vs. RR vs. PR)
- Applying frequency weights for grouped data
- Interpreting Woolf confidence intervals
- Chi-square trend tests for ordered categorical exposures

---

## 🗂️ Repository Structure

```
Stata-data-analysis/
├── Analysis of Categorical Data.log      ← Stata output log
├── Analysis of Categorical Data.docx     ← Written assignment with interpretation
├── Data analysis Stata.docx              ← Supporting analysis document
└── README.md
```

---

## 🛠️ Tools & Requirements

- **Stata** 16 or later
- No external packages required — all commands use built-in Stata functions

---

## 🎓 Academic Context

These analyses were completed as part of the **Master of Public Health** programme at the [NUS Saw Swee Hock School of Public Health](https://sph.nus.edu.sg/). The work reflects applied epidemiological reasoning alongside technical Stata proficiency.

---

## 👩‍💻 About Me

MPH student at NUS with a clinical nursing background, focusing on health data analysis and digital mental health interventions. See my [GitHub profile](https://github.com/lfangyu443-ui) for more projects.
