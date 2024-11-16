# Data Visualization Assignments

## Table of Contents
1. Overview
2. Repository Structure
3. Module 2 - Tools
    - Excel
    - Tableau
    - Python
4. Module 3 - Data Sets
    - Personal Data
    - Government Data
    - Commercial Data
    - Learning Data
5. Module 4 - Data Set Repair
   - Government Data
   - Learning Data
6. Git Repository

## 1. Overview
This repository contains assignments focused on data visualization and exploration, utilizing various tools and techniques to create and analyze data-driven insights.

## 2. Repository Structure
The repository is structured as follows:

```
/
├── module2/
│   ├── Excel/
│   │   ├── Formula tutorial.xlsx
│   │   ├── Get more out of PivotTables.xlsx
│   │   ├── Make your first PivotTable.xlsx
│   │   ├── Take a tour.xlsx
│   ├── Tableau/
│   │   ├── Creator - Calculations.twbx
│   │   ├── Creator - Connecting to Data.twbx
│   │   ├── Creator - Getting Started.twb
│   │   ├── Creator - Mapping.twbx
│   │   ├── bestselling_books.tflx
│   │   └── sales_performance.tflx
│   └── Python/
│       └── My_First_Jupyter_Notebook.ipynb
├── module3/
│   ├── Commercial - The Look E-commerce Dataset from Google Cloud/
│   │   ├── distribution_centers.xlsx
│   │   ├── events.xlsx
│   │   ├── inventory_items.xlsx
│   │   ├── order_items.xlsx
│   │   ├── orders.xlsx
│   │   ├── products.xlsx
│   │   └── users.xlsx
│   ├── Government - NICS Firearm Background Checks from BuzzFeed/
│   │   └── nics-firearm-background-checks.csv
│   ├── Learning - Fake News Dataset from Kaggle/
│   │   └── Learning - Fake News Dataset from Kaggle.rar
│   ├── Personal - Apple Health Data/
│   │   └── Personal - Apple Health Data.rar
│   └── Dataset_Descriptions_and_Rationale.ipynb
├── module4/
│   ├── Government Data/
│   │   └── nics-firearm-background-checks-cleaned.csv
│   ├── Train Data/
│   │   └── train-cleaned.rar
├── README.md
```

## 3. Module 2 - Tools

### Excel
In this section, I completed tasks based on video training and tutorials. The following artifacts were created:
- **Take a Tour**: `Take a tour.xlsx`
- **Formula Tutorial**: `Formula tutorial.xlsx`
- **First Pivot Table**: `Make your first PivotTable.xlsx`
- **Advanced Pivot Tables**: `Get more out of PivotTables.xlsx`

### Tableau
The required creator tutorials were completed, and the resulting files are as follows:
- **Creator - Calculations**: `Creator - Calculations.twbx`
- **Creator - Connecting to Data**: `Creator - Connecting to Data.twbx`
- **Creator - Getting Started**: `Creator - Getting Started.twb`
- **Creator - Mapping**: `Creator - Mapping.twbx`
- **Creator - Getting Started with Tableau Prep Builder**: `bestselling_books.tflx`
- **Creator - Tableau Prep Conductor**: `sales_performance.tflx`

### Python
A Jupyter Notebook was created, containing:
- Markdown descriptions
- A graphic created using a Python library
- Basic Python code  
**View the notebook**: `My_First_Jupyter_Notebook.ipynb`.

## 4. Module 3 - Data Sets

### Personal Data
Contains individual health and wellness metrics.  
**Files**: `export.xml`, `export_cda.xml`.  

### Government Data
Contains monthly firearm background check records across U.S. states.  
**File**: `nics_firearm_background_checks.csv`.  

### Commercial Data
Contains e-commerce interaction, sales, and inventory data.  
**Files**: `distribution_centers.xlsx`, `events.xlsx`, `inventory_items.xlsx`, `order_items.xlsx`, `orders.xlsx`, `products.xlsx`, `users.xlsx`.  

### Learning Data
Contains labeled news articles for fake news detection.  
**Files**: `train.csv`, `test.csv`.  

## 5. Module 4 - Data Set Repair

This module involves cleaning and repairing two datasets to ensure data integrity and optimize them for analysis.

### Government Data
This dataset contains monthly firearm background check records across U.S. states, sourced from BuzzFeed’s **NICS Firearm Background Checks** dataset.  
**File**: `nics_firearm_background_checks.csv`  

**Data Cleaning and Issue Mitigation**:

- **Missing Data**:
   - **Issue**: Several columns, including `permit_recheck`, `other`, and `returned_handgun`, contained missing values, which could lead to inaccuracies in analysis.
   - **Mitigation**: Missing values were filled with `0`, assuming that the absence of data indicates no activity in those categories. This approach ensures consistency in the dataset without distorting analysis results.

- **Sparse Data in Specific Columns**:
   - **Issue**: Certain columns, such as `rentals_handgun` (0.96% non-zero), `rentals_long_gun` (0.90% non-zero), and `return_to_seller_other` (3.39% non-zero), contained very few non-zero values, contributing minimally to analysis.
   - **Mitigation**: These columns were removed from the dataset to streamline it and avoid potential noise, as they did not significantly impact overall insights due to their low contribution rates.

- **Redundant or Unnecessary Data (Totals Column)**:
   - **Issue**: The original `totals` column, which aggregates various transaction types, was potentially redundant as it could be derived by summing other relevant columns (e.g., `permit`, `handgun`, `long_gun`, etc.). Including a redundant column could lead to inconsistencies if not properly aligned with its components.
   - **Mitigation**: The original `totals` column was deleted. A new `totals` column was created using a formula that sums the relevant columns to ensure accuracy. This recalculated `totals` column is now consistent with the data, reducing potential errors and simplifying the dataset.

### Train Data
This dataset contains news articles used for binary classification to determine if articles are real or fake.  
**File**: `train.csv`

**Data Cleaning and Issue Mitigation**:

- **Unnecessary Column (`id`)**:
   - **Issue**: The `id` column is an arbitrary identifier that does not contribute to the model or analysis, as the model only uses the `text` and `label` columns.
   - **Mitigation**: The `id` column was removed to simplify the dataset and reduce potential data redundancy.

- **Duplicate Rows**:
   - **Issue**: 1,886 duplicate rows were found in the dataset. Duplicate rows can lead to inaccuracies in analysis by skewing results, especially in aggregate metrics.
   - **Mitigation**: The 1,886 duplicate rows were identified and removed to ensure the uniqueness and accuracy of each entry.

## 5. Git Repository
All files are organized and version-controlled using Git. The complete repository is available for viewing and cloning via GitHub.
