# Japan Influenza Surveillance Analysis (2024–2025)
#### Author
Nicole Rouleau

### Overview
This project analyzes weekly influenza surveillance data from Japan to characterize the 2024–2025 influenza season. Using publicly available government data, the analysis examines how influenza activity evolved over time, how case burden varied across demographic groups, and how surveillance intensity and antiviral resistance differed by region.
The goal of this project is to provide a clear, methodologically sound retrospective analysis rather than predictive modeling, emphasizing interpretability and appropriate use of available data.

### Data Sources
Weekly influenza surveillance reports published by Japanese public health authorities (NIID / MHLW)
Data includes:
- Weekly reported influenza cases by age group and sex
- Hospitalizations and deaths by age group
- Antiviral resistance testing results (H275Y mutation) by prefecture
- Subtype and detection summaries

All data cleaning and formatting were performed manually in Excel prior to analysis to ensure consistency across reporting tables.

### Methods
The analysis was conducted in Python using pandas, matplotlib, and seaborn. Key methodological steps include:
- Seasonal alignment of weekly data across calendar years to create a continuous 2024–2025 influenza season timeline
- Descriptive statistics to summarize overall case burden and demographic distributions
- Rate-of-change analysis using week-over-week and rolling percent changes to identify periods of rapid acceleration and decline
- Regional comparison using prefecture-level summaries to contextualize surveillance intensity and antiviral resistance
- Forecasting was intentionally omitted because the full season was already observed; producing predictions on known outcomes would not provide meaningful insight.

### Key Findings
The 2024–2025 influenza season exhibited a rapid early surge, followed by a sharp and sustained decline rather than a gradual taper. Growth-rate analysis showed that transmission accelerated quickly and then transitioned into negative week-over-week change for the remainder of the season. Case burden varied by age group and sex, with certain demographic groups contributing disproportionately to total reported cases. Surveillance intensity varied widely by prefecture, emphasizing the importance of interpreting regional patterns in the context of testing volume. Antiviral resistance associated with the H275Y mutation was rare and geographically limited, with most prefectures reporting no detected mutations.

### Visualizations
The project includes:
- Time-series plots of weekly case counts and growth rates
- Demographic breakdowns by age group and sex
- Supporting tables summarizing resistance and regional patterns
Visualizations prioritize clarity and accessibility, including colorblind-friendly palettes where applicable.

### Tools & Technologies
- Python (pandas, numpy)
- matplotlib & seaborn
- Plotly
- Jupyter Lab

### Why This Project Matters
Influenza surveillance data is often noisy, incomplete, and unevenly distributed across regions and populations. This project demonstrates how careful preprocessing, simple analytical techniques, and thoughtful visualization choices can produce meaningful insights without overcomplicating the analysis. The approach shown here is applicable to public health monitoring, retrospective reporting, and exploratory analysis in data-constrained settings.
