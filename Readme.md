# Tamil Nadu SIR 2026 Draft Voter Roll Impact Analysis

# Jupyter NoteBook
https://github.com/ijaihari/Tamil-Nadu-SIR-2026-Draft-Voter-Roll-Impact-Analysis/blob/main/notebooks/Tamil%20Nadu%20SIR%202026%20Draft%20Voter%20Roll%20Impact%20Analysis.ipynb

**Overview** -
This report analyzes the **Summary Intensive Revision (SIR) 2026** process in Tamil Nadu and its numerical impact on voter rolls at the **Assembly Constituency level**.

The objective is to assess whether voter roll revisions are **large enough to matter** when compared against historical **victory margins from the 2021 Assembly Election**.

This is a **data-driven impact analysis**, not an allegation-based study.

## Data Sources
The analysis uses officially published public datasets:

- Tamil Nadu Assembly Election Results (2021) https://en.wikipedia.org/wiki/2021_Tamil_Nadu_Legislative_Assembly_election <br/>
- Electoral Roll Data (SSR 2025 – pre-SIR) https://www.elections.tn.gov.in/ACwise_Gendercount_06012025.aspx  <br/>
- Draft Electoral Roll Data (SIR 2026 – post-revision) https://www.elections.tn.gov.in/ACwise_Gendercount_19122025.aspx

All datasets were cleaned, validated, and aligned at the **Assembly Constituency** level.

# Key State-Level Numbers

| Metric | Count |
|------|------|
| Total voters (2021 Assembly Roll) | **6.29 crore** |
| Total voters (SSR 2025 – pre-SIR) | **6.36 crore** |
| Total voters (Draft Roll after SIR 2026) | **5.43 crore** |
| **Net voters removed (SIR 2026)** | ~ 97 lakh |

**One-line takeaway:**  
Tamil Nadu’s draft electoral roll shows a net reduction of **~ 97 lakh voters** after SIR 2026.

# Analytical Framework

The analysis is built on three measurable quantities:

1. **Victory Margin (2021)**  
   Votes that decided the winner in each constituency.

2. **Not Voted (2021)**  
   Registered voters who did not vote — used as a historical baseline.

3. **Removed Voters (2026)**  
   Net difference between eligible voters in 2021 and the draft roll after SIR 2026.

# Core Question
Are voter roll changes large enough to exceed the margin that decided the previous election?

# Impact Classification Method

Each constituency is classified by comparing **Removed Voters (2026)** against:
- Victory Margin (2021)
- Not Voted (2021)

# Risk Levels

| Risk Level | Interpretation |
|----------|---------------|
| No Removal / Increase | Voter count increased or remained stable |
| Low Impact | Removed voters < victory margin |
| Moderate Impact | Removed voters > not-voted baseline but < victory margin |
| High Impact | Removed voters > victory margin |
| Critical Impact | Removed voters > victory margin **and** > not-voted baseline |

This classification identifies **numerical sensitivity**, not intent or outcome.

## Key Findings (Constituency Level)

- **159 out of 234 constituencies** fall under **High or Critical Impact**
- In many constituencies, **removed voters exceed the votes required to win**
- Voter roll changes are **not uniform across the state**
- Removals are **concentrated in specific regions**, rather than evenly distributed

## High Impact Constituencies (Top 50)
- A total of **159 constituencies** are classified as High Impact.  
- The table above shows the **Top 50 by removed voter count**.  
- The complete list is available here: [high_impact_constituencies.csv](result%20data/high_impact_constituencies.csv)


| S.No | AC No | Constituency | Victory Margin (2021) | Removed Voters (2026) | High Impact Probability |
|----:|------:|-------------|----------------------:|----------------------:|------------------------:|
| 1 | 27 | Shozhinganallur | 35,405 | 214,882 | 1.000000 |
| 2 | 30 | Pallavaram | 37,783 | 141,527 | 0.999997 |
| 3 | 7 | Maduravoyal | 31,721 | 126,788 | 0.999995 |
| 4 | 26 | Velachery | 4,352 | 124,579 | 1.000000 |
| 5 | 28 | Alandur | 40,571 | 121,847 | 0.999968 |
| 6 | 31 | Tambaram | 36,824 | 121,308 | 0.999997 |
| 7 | 22 | Virugampakkam | 18,367 | 116,568 | 0.999999 |
| 8 | 12 | Perambur | 54,976 | 115,761 | 0.999997 |
| 9 | 14 | Villivakkam | 37,237 | 112,622 | 0.999993 |
|10 | 24 | Thiyagarayanagar | 137 | 105,542 | 1.000000 |
|11 | 20 | Thousand Lights | 32,462 | 98,703 | 0.999921 |
|12 | 13 | Kolathur | 70,384 | 94,356 | 0.999846 |
|13 | 23 | Saidapet | 29,408 | 92,544 | 0.999932 |
|14 |114 | Tiruppur (South) | 4,709 | 91,201 | 0.999999 |
|15 | 25 | Mylapore | 12,633 | 88,976 | 0.999995 |
|16 | 6 | Ambattur | 16,448 | 87,422 | 0.999901 |
|17 | 46 | Hosur | 26,218 | 83,854 | 0.999782 |
|18 | 10 | Egmore | 53,287 | 82,819 | 0.999642 |
|19 | 83 | Tiruchendur | 13,721 | 79,935 | 0.999391 |
|20 | 58 | Salem North | 11,400 | 77,226 | 0.999323 |
|21 | 59 | Salem South | 20,431 | 76,912 | 0.999252 |
|22 | 95 | Karur | 70,654 | 76,421 | 0.999174 |
|23 | 84 | Srivaikuntam | 6,509 | 73,484 | 0.999013 |
|24 | 62 | Erode East | 56,496 | 72,614 | 0.998891 |
|25 | 61 | Erode West | 11,230 | 71,034 | 0.998743 |
|26 |102 | Kovilpatti | 31,187 | 69,812 | 0.998501 |
|27 |101 | Vilathikulam | 14,151 | 69,184 | 0.998366 |
|28 | 99 | Thoothukkudi | 65,019 | 68,422 | 0.998192 |
|29 | 72 | Aranthangi | 20,621 | 65,341 | 0.997881 |
|30 | 71 | Pudukkottai | 17,823 | 64,102 | 0.997702 |
|31 |107 | Uthangarai | 3,811 | 62,244 | 0.997455 |
|32 |103 | Sattur | 17,916 | 61,391 | 0.997214 |
|33 |152 | Vriddhachalam | 19,058 | 60,188 | 0.996912 |
|34 |156 | Cuddalore | 8,734 | 59,861 | 0.996785 |
|35 |164 | Ramanathapuram | 14,118 | 57,230 | 0.996220 |
|36 | 36 | Kancheepuram | 12,784 | 56,638 | 0.996103 |
|37 | 37 | Chengalpattu | 29,148 | 55,321 | 0.995873 |
|38 | 47 | Krishnarayapuram | 8,431 | 53,109 | 0.995402 |
|39 | 97 | Manamadurai | 23,018 | 52,371 | 0.995104 |
|40 | 80 | Nanguneri | 3,373 | 51,982 | 0.994988 |
|41 | 82 | Cheranmahadevi | 12,837 | 50,774 | 0.994755 |
|42 | 48 | Ulundurpettai | 9,335 | 49,618 | 0.994512 |
|43 | 108 | Gudiyatham | 19,329 | 48,944 | 0.994104 |
|44 | 68 | Kumbakonam | 21,276 | 47,829 | 0.993856 |
|45 | 75 | Orathanadu | 6,243 | 46,991 | 0.993602 |
|46 | 89 | Aruppukkottai | 14,782 | 45,870 | 0.993337 |
|47 | 121 | Sankarankovil | 9,211 | 44,905 | 0.993101 |
|48 | 133 | Viluppuram | 18,204 | 44,012 | 0.992884 |
|49 | 52 | Bargur | 15,506 | 43,176 | 0.992643 |
|50 | 144 | Neyveli | 11,873 | 42,589 | 0.992417 |

> In these constituencies, voter removals are significantly larger than the margin that decided the last election.

# Visual Analysis Summary

### Chart 1: Victory Margin vs Removed Voters
**Purpose:**  
To identify constituencies where voter removals exceed historical victory margins.

![Victory Margin vs Removed Voters](result%20data/victory_margin%20vs%20removed_voters.png)

**Key observation:**  
Many constituencies lie above the victory margin threshold, indicating numerical sensitivity.

### Chart 2: High-Impact Constituencies (Bar Comparison)
**Purpose:**  
Side-by-side comparison of removed voters vs victory margin.

![High Impact Constituencies](result%20data/high_impact_constituencies.png)

**Key observation:**  
In high-impact seats, the removed voter count consistently exceeds the winning margin.

### Chart 3: Distribution of Risk Levels
**Purpose:**  
To understand how impact is spread across the state.

![Risk Distribution](result%20data/distrubution_of_voter_roll_impact_risk.png)

**Key observation:**  
A majority of constituencies fall under **High Impact**, with a smaller but critical set under **Critical Impact**.

# Logistic Regression (Validation Analysis)

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

# Final Conclusion

When voter roll removals exceed historical victory margins, constituencies become **numerically sensitive** to roll revisions.

The combined visual analysis and statistical modeling lead to a consistent conclusion:

> **Large voter roll changes can matter most in closely contested constituencies, especially when voter growth does not offset removals.**

This analysis **does not claim election outcomes were affected**.  
It identifies **where accuracy and care in voter roll revision are most critical**.

Complete analysis with charts, tables, and methodology.

# Skills Demonstrated
- Public data analysis  
- Web scraping & data collection  
- Data cleaning and transformation  
- Exploratory Data Analysis (EDA)  
- Statistical modeling  
- Responsible analysis of sensitive datasets  

# Disclaimer
This is an independent analytical exercise based on publicly available data.  
It aims to improve **transparency and numerical understanding**, not to assign intent or blame.
