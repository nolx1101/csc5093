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
   - Train Data
6. Module 4 - Data Visualization
   - Government Data
7. Module 5 - Foundational Element Creations
   - Excel
   - Python
8. Module 5 - Design Principles: Space, Motion, Value, and Color
   - Python
9. Git Repository

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
│   │   └── nics-visualizations-yearly-and-type.twbx
│   ├── Train Data/
│   │   └── train-cleaned.rar
├── module5/
│   ├── Excel/
│   │   └── firearm_visualizations.xlsx
│   ├── Python/
│   │   ├── Firearm_Data_Visualizations.ipynb
│   │   ├── trend_over_time.png
│   │   ├── state_comparison.png
│   │   ├── firearm_types_california.png
│   │   ├── Ecommerce_Visualizations.ipynb
│   │   ├── yearly_revenue.png
│   │   └── delivery_time_distribution.png
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
**File**: `nics_firearm_background_checks-cleaned.csv`  

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
**File**: `train-cleaned.csv`

**Data Cleaning and Issue Mitigation**:

- **Unnecessary Column (`id`)**:
   - **Issue**: The `id` column is an arbitrary identifier that does not contribute to the model or analysis, as the model only uses the `text` and `label` columns.
   - **Mitigation**: The `id` column was removed to simplify the dataset and reduce potential data redundancy.

- **Duplicate Rows**:
   - **Issue**: 1,886 duplicate rows were found in the dataset. Duplicate rows can lead to inaccuracies in analysis by skewing results, especially in aggregate metrics.
   - **Mitigation**: The 1,886 duplicate rows were identified and removed to ensure the uniqueness and accuracy of each entry.


## 6. Module 4 - Data Visualization

### Dataset: Government Data - NICS Firearm Background Checks

**File**: `nics-firearm-background-checks-cleaned.csv`  
**Visualization Tool**: Tableau  
**Visualization File**: `nics-visualizations-yearly-and-type.twb`

This Tableau project presents two visualizations created from the NICS Firearm Background Checks dataset, focusing on trends over time and a breakdown by firearm type. These visualizations were designed to apply principles of **line**, **shape**, and **volume** to highlight different focal points.

### Visualizations

#### **1. Yearly Trends of Firearm Background Checks (Line Chart)**
- **Focal Point**: Displays the yearly trends of total firearm background checks over time.
- **Design Principle Used**: The **line principle** is employed to emphasize the direction and change in background check totals over the years.
- **Key Insights**:
  - Identifies trends in firearm background checks over time, including peaks and declines.
  - Helps understand year-to-year fluctuations in background checks.

#### **2. Firearm Types Breakdown (Stacked Bar Chart)**
- **Focal Point**: Highlights the contribution of different firearm types (`handgun`, `long_gun`, `other`) to the overall background checks.
- **Design Principle Used**: The **shape/volume principle** is used in the stacked bar chart to visually compare the proportions of firearm types.
- **Key Insights**:
  - Allows comparison of the relative volume of firearm background checks for each type.
  - Shows how firearm types contribute to yearly or statewide totals.

### Note on Data Cleaning

- **Date Format**: The date format in the `month` column was standardized to ensure consistency and compatibility with Tableau visualizations.

## 7. Module 5 - Foundational Element Creations

### Firearm Data Visualizations
This module focuses on creating foundational visualizations of government firearm background check data using Excel and Python. The visualizations explore yearly trends, state-level comparisons, and firearm type breakdowns.

**Data Source**:
- `nics-firearm-background-checks-cleaned.csv`

**Tools**:
- Excel
- Python (Jupyter Notebook)

### Tasks Performed

#### **1. Visualizations in Excel**
- **Trends Over Time (Line Chart)**:
  - Aggregated yearly firearm background checks using a Pivot Table.
  - Created a line chart to visualize trends across all years.
- **State Comparison (Clustered Bar Chart)**:
  - Compared state-level firearm background checks across all years using a Pivot Table.
  - Created a clustered bar chart.
- **Firearm Types in California (Clustered Column Chart)**:
  - Compared `Handgun`, `Long Gun`, and `Other` firearm checks within California.
  - Created a clustered column chart.

**Output**:
- `firearm_visualizations.xlsx`:
  - Sheet: `Trends Over Time`
  - Sheet: `State Comparison`
  - Sheet: `Firearm Types in California`

#### **2. Visualizations in Python**
- **Yearly Firearm Trends (Line Chart)**:
  - Visualized yearly firearm background checks across all years.
  - **Title**: `Total Firearm Background Checks Over Time`.
- **State-Wise Firearm Totals for 2023 (Clustered Bar Chart)**:
  - Focused on state-level totals for 2023 only.
  - **Title**: `State-Wise Firearm Background Checks (2023)`.
- **Firearm Types in California (Clustered Column Chart)**:
  - Compared firearm types in California.
  - **Title**: `Firearm Types in California`.

**Output**:
- Jupyter Notebook: `Firearm_Data_Visualizations.ipynb`
- Visualization Files:
  - `trend_over_time.png`
  - `state_comparison.png`
  - `firearm_types_california.png`

### Summary
This module highlights the use of Excel and Python to create visualizations for firearm background checks, leveraging Pivot Tables and Matplotlib for insights into trends, state comparisons, and firearm type breakdowns.

## 8. Module 5 - Design Principles: Space, Motion, Value, and Color

This module focuses on applying design principles - **space**, **motion**, **value**, and **color** - to create meaningful data visualizations using Python. Two visualizations were created from the e-commerce dataset to effectively demonstrate these principles.

### **Visualizations**

1. **Yearly Revenue Over Time (Line Chart)**:
   - **Focus**: Value and Motion.
   - **Description**: This line chart highlights yearly revenue trends, illustrating how revenue evolves over time.
     - **Value**: The Y-axis represents revenue in dollars, quantifying annual performance.
     - **Motion**: The progression of years along the X-axis creates an illusion of motion, emphasizing growth trends.
   - **Output**: `yearly_revenue.png`

2. **Delivery Time Distribution (Histogram)**:
   - **Focus**: Space and Value.
   - **Description**: This histogram shows the frequency of delivery times (in days), identifying common delivery durations and highlighting outliers.
     - **Space**: Evenly spaced bins ensure a clean visualization of delivery times without overlaps or gaps.
     - **Value**: The Y-axis quantifies the frequency of deliveries, providing actionable insights for optimization.
   - **Output**: `delivery_time_distribution.png`

### **Notebook**
- **`Ecommerce_Visualizations.ipynb`**: Contains Python code and visualizations created using design principles.

## 9. Git Repository
All files are organized and version-controlled using Git. The complete repository is available for viewing and cloning via GitHub.
