# GLP-1 Medication Use, Income, and Healthcare Affordability

## Project Overview

This project explores how GLP-1 medication use has changed over time and how income and healthcare affordability relate to access to these medications. GLP-1 medications include Ozempic, Wegovy, and Mounjaro. We examined national health survey data to better understand patterns in prescription use and healthcare affordability from 2020 through 2024.

## Research Questions

1. How has the use of GLP-1 medications increased or decreased over the past several years?
2. Does income affect access to GLP-1 medications?
3. How has healthcare and prescription affordability changed as GLP-1 use has increased?

## Data Sources

We selected three publicly available U.S. health datasets for this project:

| Dataset | What it contains | Role in this project |
| --- | --- | --- |
| **Medical Expenditure Panel Survey (MEPS)** | Information on healthcare use, prescription medicines, costs, and household characteristics in the United States. | Used to examine GLP-1 prescription trends from **2020–2024** and compare prescription use across income groups in **2023**. |
| **National Health Interview Survey (NHIS)** | Survey information about health, healthcare access, insurance, and difficulties affording care. | Used to examine changes in the ability to afford prescriptions and medical care from **2020–2024**. |
| **Behavioral Risk Factor Surveillance System (BRFSS)** | Survey information about health behaviors, chronic conditions, and preventive care among U.S. adults. | Selected as an additional dataset relevant to health and access questions. **The findings summarized below do not include a separate BRFSS analysis.** |

For the 2023 income analysis, we used the **MEPS Full Year Consolidated** file and **Prescribed Medicines** file. Records were matched by person ID to compare recorded GLP-1 prescriptions across five income categories: Poor/Negative, Near Poor, Low Income, Middle Income, and High Income.

## Tools and Methods

- **Excel:** Organized and combined data, matched person records, and prepared the income variables.
- **Tableau:** Explored trends and created visualizations.
- **Excel Solver:** Estimated a logistic regression to compare GLP-1 prescription use across income categories.
- **ChatGPT:** Assisted with combining annual datasets, organizing records, and explaining analysis steps.

To avoid double-counting people with multiple prescriptions, we organized the medication data so each person was counted once within each year.

## Key Findings

### 1. GLP-1 Medication Use Increased

Our preliminary MEPS analysis estimated the following numbers of GLP-1 users:

| Year | Estimated Users |
| --- | ---: |
| 2020 | 3.09 million |
| 2021 | 4.17 million |
| 2022 | 5.50 million |
| 2023 | 8.81 million |
| 2024 | 11.69 million |

These preliminary estimates suggest that GLP-1 use increased by approximately **278.5%** from 2020 to 2024. The largest year-to-year increase was between 2022 and 2023, at approximately **60.2%**.

### 2. Income and GLP-1 Prescription Use

Using 2023 MEPS data, we compared recorded GLP-1 prescription use across five income groups. Rates ranged from **2.49% to 3.45%**. The Poor/Negative income group had the highest observed rate, while the Low Income group had the lowest.

We also ran a logistic regression with High Income as the reference category. The overall likelihood-ratio test had a **p-value of 0.1363**, above the usual 0.05 cutoff. In this unweighted sample analysis, the income categories were **not statistically significantly associated** with recorded GLP-1 prescription use. This does not prove that income has no relationship with access.

### 3. Healthcare and Prescription Affordability

Our NHIS analysis found that difficulties affording care increased between 2020 and 2024:

| Affordability Measure | 2020 | 2024 |
| --- | ---: | ---: |
| Adults unable to afford prescriptions | 5.68% | 6.30% |
| Adults unable to afford medical care | 6.63% | 7.39% |

Healthcare affordability challenges increased during the same period that estimated GLP-1 use grew. **These parallel trends do not establish that GLP-1 medications caused affordability problems.** NHIS measures reported affordability difficulties rather than actual prescription spending in this analysis.

## Limitations

- The findings are preliminary and depend on how medications and survey records were identified and combined.
- Recorded prescriptions are not a direct measure of every person's ability to access or obtain GLP-1 medications.
- The 2023 income regression was performed on an **unweighted MEPS sample**; its significance test should not be interpreted as a survey-design-adjusted national estimate.
- The NHIS affordability findings describe broad healthcare and prescription affordability, not GLP-1-specific costs.
- BRFSS is described as a selected source, but no separate BRFSS findings are presented here.
- Observed trends and associations do not establish cause and effect.

## Conclusion

Our project found a substantial increase in estimated GLP-1 medication use between 2020 and 2024. The 2023 income analysis showed some differences across income groups, but those differences were not statistically significant in our unweighted logistic regression. At the same time, NHIS results showed growing difficulties affording prescriptions and medical care. Together, these findings highlight the importance of studying medication use alongside income, insurance, and healthcare affordability.

## Data Source Websites

- [MEPS — Agency for Healthcare Research and Quality](https://meps.ahrq.gov/)
- [NHIS — National Center for Health Statistics](https://www.cdc.gov/nchs/nhis/)
- [BRFSS — Centers for Disease Control and Prevention](https://www.cdc.gov/brfss/)
