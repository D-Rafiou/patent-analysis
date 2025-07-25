# patent-data-analysis
Patent Grant Time Analysis
An analysis of U.S. patent grant times using 2023 patent data to examine how technology field and assignee type influence patent processing duration.
Overview
This project explores two key questions:

Do certain fields have faster patent grant times than others?
Do organizations receive patents faster than individual inventors?

Data

Source: 2023 U.S. patent data (CSV format)
Key Variables:

years_to_grant: Time from application to grant
first_wipo_field_title: Field classification
assignee_ind: Individual (1) vs Organization (0) indicator



Methodology
Data Preparation

Created assignee_type variable mapping individuals and organizations
Calculated years_to_grant from application and grant years
Focused on top 10 patent fields (>7,000 patents each)
Balanced dataset for assignee type comparison

Analysis Approach

Field Analysis: Bar plots and box plots comparing grant times across fields
Assignee Analysis: Balanced sampling and t-test to compare individuals vs organizations
Portfolio Analysis: Examined field preferences by assignee type

Key Findings
Field Impact ✅

Digital fields fastest: Telecommunications, Semiconductors, Computer Technology (2.2-2.5 years)
Regulated fields slowest: Pharmaceuticals, Medical Technology (>3.2 years)
Significant variation supports complexity-based processing hypothesis

Assignee Type Impact ❌

No significant difference between individuals and organizations (p > 0.05)
Balanced sampling confirmed consistent processing times
Portfolio differences explain apparent contradictions

Field Portfolio Effect 🔍

Individuals: Focus on mechanical, medical, and engineering fields
Organizations: Concentrate on digital and communication technologies
Field specialization, not applicant type, drives grant time differences

Technologies Used

Python: pandas, seaborn, matplotlib, scipy
Statistical Methods: t-tests, descriptive statistics, data visualization

Files

2023.csv: Patent data (not included - source from USPTO)
analysis.ipynb : main notebook file used for the whole project
Analysis includes data preparation, visualization, and statistical testing

Conclusion
Patent processing time reflects complexity rather than applicant resources. The U.S. patent system demonstrates consistent examination standards across individual inventors and organizations, with field-specific regulatory and technical demands being the primary factor in grant duration.