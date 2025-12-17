# Looker_Dashboard_Visualization

This mock project demonstrates an end-to-end data workflow where data is collected through Jotform, stored and cleaned in Google Sheets, and visualized using Looker dashboards. The project emphasizes data accuracy, automation, and clear reporting.

Architecture & Workflow

Data Collection
Data is collected via Jotform with built-in validations to reduce input errors and improve accuracy at the source.

Data Storage
Submissions automatically populate Google Sheets in Jotform_Raw, which stores unedited source data. A second sheet, Jotform_Clean, highlights the transformation from raw input to structured output.

Data Cleaning
Cleaning is performed using Google Sheets formulas such as ARRAYFORMULA, PROPER, and TOPCOL to standardize text, remove duplicates, handle missing values, and ensure consistent capitalization (e.g., LaRRy → Larry) 

Visualization
Cleaned data is connected to Looker, where dashboards present KPIs, charts, tables, and progress bars. Conditional formatting and clear visual hierarchy support quick insight discovery.

Assumptions & Limitations

Handles common formatting issues; complex anomalies may require manual review.

Changes to sheet structure or column names may impact Looker visuals.( deletion, etc)

Performance may degrade with very large datasets due to platform limits.
