# Tamil Nadu SIR 2026 Draft Voter Roll Impact Analysis

## Overview
This report analyzes the **Summary Intensive Revision (SIR) 2026** process in Tamil Nadu and its numerical impact on voter rolls at the **Assembly Constituency level**.

The objective is to assess whether voter roll revisions are **large enough to matter** when compared against historical **victory margins from the 2021 Assembly Election**.

> This is a **data-driven impact analysis**, not an allegation-based study.

---

## Data Sources
The analysis uses officially published public datasets:

- Tamil Nadu Assembly Election Results (2021)
- Electoral Roll Data (SSR 2025 – pre-SIR)
- Draft Electoral Roll Data (SIR 2026 – post-revision)

All datasets were cleaned, validated, and aligned at the **Assembly Constituency** level.

---

## Key State-Level Numbers

| Metric | Count |
|------|------|
| Total voters (2021 Assembly Roll) | **6.29 crore** |
| Total voters (SSR 2025 – pre-SIR) | **6.36 crore** |
| Total voters (Draft Roll after SIR 2026) | **5.43 crore** |
| **Net voters removed (SIR 2026)** | **97.3 lakh** |

**One-line takeaway:**  
Tamil Nadu’s draft electoral roll shows a net reduction of **~0.97 crore voters** after SIR 2026.

---

## Analytical Framework

The analysis is built on three measurable quantities:

1. **Victory Margin (2021)**  
   Votes that decided the winner in each constituency.

2. **Not Voted (2021)**  
   Registered voters who did not vote — used as a historical baseline.

3. **Removed Voters (2026)**  
   Net difference between eligible voters in 2021 and the draft roll after SIR 2026.

### Core Question
> Are voter roll changes large enough to exceed the margin that decided the previous election?

---

## Impact Classification Method

Each constituency is classified by comparing **Removed Voters (2026)** against:
- Victory Margin (2021)
- Not Voted (2021)

### Risk Levels

| Risk Level | Interpretation |
|----------|---------------|
| No Removal / Increase | Voter count increased or remained stable |
| Low Impact | Removed voters < victory margin |
| Moderate Impact | Removed voters > not-voted baseline but < victory margin |
| High Impact | Removed voters > victory margin |
| Critical Impact | Removed voters > victory margin **and** > not-voted baseline |

This classification identifies **numerical sensitivity**, not intent or outcome.

---

## Key Findings (Constituency Level)

- **159 out of 234 constituencies** fall under **High or Critical Impact**
- In many constituencies, **removed voters exceed the votes required to win**
- Voter roll changes are **not uniform across the state**
- Removals are **concentrated in specific regions**, rather than evenly distributed

---

## High-Impact Constituencies (Sample)

| Constituency | Victory Margin (2021) | Removed Voters (2026) | Risk Level |
|-------------|----------------------|-----------------------|-----------|
| Shozhinganallur | 35,405 | 214,882 | High Impact |
| Pallavaram | 37,783 | 141,527 | High Impact |
| Maduravoyal | 31,721 | 126,788 | High Impact |
| Velachery | 4,352 | 124,579 | High Impact |
| Anna Nagar | 27,445 | 123,955 | Critical Impact |

> In these constituencies, voter removals are significantly larger than the margin that decided the last election.

Full lists are available in:
- `result data/final_analytical_dataset.csv`
- `result data/high_impact_constituencies.csv`
- `result data/total_critical_high_impact.csv`

---

## Visual Analysis Summary

### Chart 1: Victory Margin vs Removed Voters
**Purpose:**  
To identify constituencies where voter removals exceed historical victory margins.

![Victory Margin vs Removed Voters](result%20data/victory_margin_vs_removed_voters.png)

**Key observation:**  
Many constituencies lie above the victory margin threshold, indicating numerical sensitivity.

---

### Chart 2: High-Impact Constituencies (Bar Comparison)
**Purpose:**  
Side-by-side comparison of removed voters vs victory margin.

![High Impact Constituencies](result%20data/high_impact_constituencies.png)

**Key observation:**  
In high-impact seats, the removed voter count consistently exceeds the winning margin.

---

### Chart 3: Distribution of Risk Levels
**Purpose:**  
To understand how impact is spread across the state.

![Risk Distribution](result%20data/distribution_of_voter_roll_impact_risk.png)

**Key observation:**  
A majority of constituencies fall under **High Impact**, with a smaller but critical set under **Critical Impact**.

---

## Logistic Regression (Validation Analysis)

A logistic regression model was used to **validate impact classification**, not to predict election outcomes.

### Model Objective
Identify constituencies where **removed voters exceed victory margins**.

### Key Influencing Factors
- **Removed voters (absolute count)** – strongest positive influence
- **Roll change percentage** – strong influence
- **Not voted (2021)** – moderate influence
- **Victory margin (2021)** – strong negative influence

### Model Result
- High classification accuracy
- Confirms that **voter removal size** is the primary driver of impact risk

---

## Final Conclusion

When voter roll removals exceed historical victory margins, constituencies become **numerically sensitive** to roll revisions.

The combined visual analysis and statistical modeling lead to a consistent conclusion:

> **Large voter roll changes can matter most in closely contested constituencies, especially when voter growth does not offset removals.**

This analysis **does not claim election outcomes were affected**.  
It identifies **where accuracy and care in voter roll revision are most critical**.

---

## Attached Report
📄 **TN_SIR_2026_Impact_Analysis.pdf**  
Complete analysis with charts, tables, and methodology.

---

## Skills Demonstrated
- Public data analysis  
- Web scraping & data collection  
- Data cleaning and transformation  
- Exploratory Data Analysis (EDA)  
- Statistical modeling  
- Responsible analysis of sensitive datasets  

---

## Disclaimer
This is an independent analytical exercise based on publicly available data.  
It aims to improve **transparency and numerical understanding**, not to assign intent or blame.
