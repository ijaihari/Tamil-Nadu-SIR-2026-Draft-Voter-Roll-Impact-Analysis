# Tamil Nadu SIR Voter Roll Revision Impact Analysis (Data Analytics Project)

Final Analysis Notebook - 
https://github.com/ijaihari/Tamil-Nadu-SIR-2025-Draft-Voter-Roll-Impact-Analysis/blob/main/notebooks/final_analysis.ipynb

## Project Overview
This project analyzes voter roll revisions under the **Tamil Nadu Special Intensive Revision (SIR) 2025** and evaluates whether these changes are large enough to matter when compared to **victory margins from the 2021 Assembly Election**.

The analysis focuses on **numerical impact**, not intent, and aims to identify constituencies where voter roll changes could potentially influence election outcomes.


## Core Idea
**Victory margin** acts as a threshold to assess whether structural voter roll changes are large enough to influence electoral outcomes.

## Data Sources
- Tamil Nadu Assembly Election Results (2021)
- Voter Roll Data (SSR 2021)
- Voter Roll Data (SIR 2025 – AC-wise)
- Official sources from the Election Commission of Tamil Nadu


## Methodology
1. Extracted constituency-level election results and voter roll data
2. Calculated victory margins for the 2021 election
3. Computed voter roll changes between 2021 and 2025
4. Compared voter removals against:
   - Victory margin (outcome sensitivity)
   - Not voted voters in 2021 (context)
5. Classified constituencies into risk levels based on numerical impact


## Risk Levels Explained
- **Low Impact** – Roll changes unlikely to affect results  
- **Moderate Impact** – Roll changes noticeable but below victory margin  
- **High Impact** – Removed voters exceed victory margin  
- **Critical Impact** – Removed voters exceed both margin and historical non-voters  
- **No Removal / Increase** – Voter count stable or increased  


## Key Findings
- **159 out of 234 constituencies** fall under the **High Impact** category
- The winning side in 2021 secured **133 seats**, with **118 required** to form a government
- A large number of seats are numerically sensitive to voter roll changes


## Visual Analysis
The project includes:
- Victory Margin vs Removed Voters scatter plots
- Bubble charts with turnout context
- Combined column charts for high-impact constituencies
- Risk-level distribution charts

All visualizations are created using **Matplotlib**.


## Tools & Technologies
- Python (Pandas, Matplotlib)
- SQL (SQLite)
- Jupyter Notebook
- Web scraping (BeautifulSoup)

## Conclusion
In several constituencies, voter roll removals are higher than the victory margin from the 2021 election, which means there may be a chance for election results to change in those seats.  
This does not confirm outcome changes, but it highlights the importance of **accurate voter roll revision in closely contested elections**.


## Disclaimer
This project is a **data analytics exercise** based on publicly available information.  
It does **not** claim election irregularities or intent, and all conclusions are drawn purely from numerical comparisons.



## Sources

https://en.wikipedia.org/wiki/2021_Tamil_Nadu_Legislative_Assembly_election <br/>
https://www.elections.tn.gov.in/ACwise_Gendercount_06012025.aspx  <br/>
https://www.elections.tn.gov.in/ACwise_Gendercount_19122025.aspx