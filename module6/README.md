# Module 6: Firearm Checks Dashboard

This directory contains the files for the Module 6 assignment in the Data Visualization course. The focus of this module is building an interactive Tableau dashboard using firearm background check data.

## File Contents
1. **Firearm_Checks_Dashboard.twb**
   - Tableau workbook containing:
     - **Trend Line:**
       - Displays total firearm background checks over time alongside YoY Growth (%).
     - **Map:**
       - Shows geographic distribution of firearm background checks by state, with a filter for year.
     - **Category Breakdown:**
       - Explores the contribution of handgun, long gun, and other checks over time.
     - **Interactive Dashboard:**
       - Combines all three visualizations with filters for state and year.

2. **Details_Notebook.ipynb**
   - Jupyter Notebook summarizing:
     - The design choices for the dashboard.
     - Steps taken to create each visualization.
     - Key insights from the visualizations.

3. **README.md**
   - This file, summarizing the contents of the module6 directory.

## Notes
- The data used in this dashboard (`nics-firearm-background-checks-cleaned.csv`) is located in the `data/` directory and was cleaned in a previous module. Details of the cleaning process are documented in the `data/README.md` file.

## Directory Structure
```
/
module6/
├── data/
│   ├── nics-firearm-background-checks-cleaned.csv
│   ├── README.md
├── Firearm_Checks_Dashboard.twb
├── Details_Notebook_Module6.ipynb
├── README.md
```
