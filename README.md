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
   - Firearm Data Visualizations (Excel and Python)
8. Module 5 - Design Principles: Space, Motion, Value, and Color
   - E-commerce Visualizations (Python)
9. Module 6 - Interactive Dashboard
   - Tableau
10. Module 7 - Visual Resume
11. Module 7 - Final Presentation Story Outline
12. Module 8 - Final Presentation
13. Git Repository

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
│   ├── data/
│   │   ├── nics-firearm-background-checks-cleaned.csv
│   │   ├── order_items.xlsx
│   │   └── README.md
│   ├── Design_Principles/
│   │   ├── Ecommerce_Visualizations.ipynb
│   │   ├── yearly_revenue.png
│   │   ├── delivery_time_distribution.png
│   │   └── README.md
│   ├── Foundational_Element_Creations/
│   │   ├── firearm_visualizations.xlsx
│   │   ├── Firearm_Data_Visualizations.ipynb
│   │   ├── trend_over_time.png
│   │   ├── state_comparison.png
│   │   ├── firearm_types_california.png
│   │   └── README.md
├── module6/
│   ├── data/
│   │   ├── nics-firearm-background-checks-cleaned.csv
│   │   └── README.md
│   ├── Firearm_Checks_Dashboard.twb
│   ├── Details_Notebook_Module6.ipynb
│   └── README.md
├── module7/
│   ├── data/
│   │   ├── Resume.xlsx
│   │   ├── Border_Crossing_Entry_Data.csv
│   │   └── README.md
│   ├── Visual_Resume.twbx
│   ├── Details_Visual_Resume_Module7.ipynb
│   ├── Border_Crossing_Analysis.twb
│   ├── Module 7 Final Presentation Story Outline.docx
│   └── README.md
├── module8/
│   ├── data/
│   │   ├── Border_Crossing_Entry_Data.csv
│   │   └── README.md
│   ├── Border_Crossing_Analysis.twbx
│   ├── Border Crossing Entry Data Analysis.docx
│   ├── Border Crossing Analysis Presentation.pptx
│   ├── Border Crossing Analysis Video.mp4
│   └── README.md
└── README.md
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

This module focuses on creating foundational visualizations using Excel and Python. Government firearm background check data is analyzed to explore yearly trends, state-level comparisons, and firearm type breakdowns.

- **Excel Visualizations:**
  - **Trends Over Time (Line Chart):** Aggregated yearly firearm background checks.
  - **State Comparison (Bar Chart):** Compared state-level firearm background checks.
  - **Firearm Types in California (Column Chart):** Compared handgun, long gun, and other checks.
  - **File:** `firearm_visualizations.xlsx`.

- **Python Visualizations:**
  - **Yearly Firearm Trends (Line Chart):** Visualized yearly firearm background checks.
  - **State-Wise Firearm Totals (Bar Chart):** Focused on state-level totals for 2023.
  - **Firearm Types in California (Column Chart):** Compared firearm types in California.
  - **Files:**
    - `trend_over_time.png`
    - `state_comparison.png`
    - `firearm_types_california.png`.

Key files:
- **Firearm_Data_Visualizations.ipynb**: Notebook containing Python code and outputs for creating foundational visualizations of firearm background check data.
- **firearm_visualizations.xlsx**: Excel file with foundational visualizations.

## 8. Module 5 - Design Principles: Space, Motion, Value, and Color

This module focuses on applying design principles - **space**, **motion**, **value**, and **color** - to create meaningful data visualizations. The E-commerce dataset was used to develop insightful and visually engaging representations with Python.

- **Yearly Revenue Over Time (Line Chart):**
  - Demonstrates motion (progression of years) and value (revenue trends).
  - **File:** `yearly_revenue.png`.

- **Delivery Time Distribution (Histogram):**
  - Demonstrates space (proper bin spacing) and value (delivery frequency).
  - **File:** `delivery_time_distribution.png`.

Key files:
- **Ecommerce_Visualizations.ipynb**: Notebook containing the Python code and visualizations demonstrating the application of design principles.
- **order_items.xlsx**: Dataset used for E-commerce visualizations.

## 9. Module 6 - Interactive Dashboard
This module focuses on creating an interactive dashboard in Tableau, utilizing firearm background check data for the visualizations.
The dashboard integrates the following:
- **Trend Line:** Displays total firearm background checks over time alongside YoY Growth (%).
- **Map:** Shows the geographic distribution of firearm background checks by state, with filtering options.
- **Category Breakdown:** Explores the contribution of different firearm types (handgun, long gun, other).
- **Interactive Features:** Includes state and year filters for synchronized visualizations.

Key files:
- **Firearm_Checks_Dashboard.twb**: Tableau workbook containing the dashboard and visualizations.
- **Details_Notebook_Module6.ipynb**: Documents the design and functionality of the dashboard.

## 10. Module 7 - Visual Resume 

This module focuses on creating a **visual resume** in Tableau, combining multiple visualizations into an interactive dashboard. The visualizations highlight education, skills, job locations, and hobbies.

### Visualizations:
1. **Gantt Chart (Education Timeline):**
   - Displays milestones in education over time.
   - Shows institutions attended, degrees obtained, and timeline information.

2. **Skills Proficiency (Bar Chart):**
   - Highlights key skills and their respective proficiency levels.

3. **Job Locations (Map):**
   - Maps job experiences with detailed information on companies, roles, and timelines.

4. **Hobbies (Bubble Chart):**
   - Visualizes hobbies with corresponding time spent, represented as bubble sizes.

### Key Files:
- **Visual_Resume.twbx**: Tableau workbook containing all visualizations.
- **Details_Visual_Resume_Module7.ipynb**: Notebook file explaining the visualizations and their creation.

## 11. Module 7 - Final Presentation Story Outline

This module outlines the final presentation for the **Border Crossing Analysis Project**, leveraging Tableau’s storytelling features. The document provides context, goals, and the sequence of visual elements used in the story.

### Context
- **Audience**: Policymakers, economists, transportation planners, and regional stakeholders.
- **Technology**: Tableau's interactive dashboard and storytelling tools.

### Goal
To analyze and present border crossing trends, regional differences, and transportation mode distributions, providing insights for infrastructure optimization and resource planning.

### Key Story Points
1. **Texas Insights**:
   - Focuses on border crossing data specific to Texas.
2. **Pedestrian Crossings**:
   - Highlights trends in pedestrian crossings across regions.
3. **U.S.-Canada Border**:
   - Analyzes northern border crossing activity.
4. **San Ysidro Port Analysis**:
   - Detailed insights into one of the busiest U.S.-Mexico ports.
5. **Peak Month: August**:
   - Explores trends in the highest activity month for crossings.

### Key Files
- **Border_Crossing_Analysis.twb**: Tableau workbook containing the analysis and stories.
- **Module 7 Final Presentation Story Outline.docx**: Document outlining the presentation story.
- **README.md**: Documentation for the project.

## 12. Module 8 - Final Presentation

### Context
The **Final Presentation** module presents an analysis of U.S. border crossing data using Tableau to create interactive visualizations and an explanatory dashboard.

### Key Components
- **Dataset**: Border Crossing Entry Data
  - *Source*: Bureau of Transportation Statistics (Data.gov)
  - *File*: `Border_Crossing_Entry_Data.csv`
- **Visualizations**:
  1. Line chart: Temporal trends in border crossings
  2. Bar chart: Comparison of crossing types by border
  3. Geographic map: State-level activity
  4. Bubble chart: Distribution of crossing types
  5. Treemap: Ports by total crossing volume
- **Deliverables**:
  - Analysis document: `Border Crossing Entry Data Analysis.docx`
  - Tableau workbook: `Border_Crossing_Analysis.twb`
  - Presentation slides: `Border Crossing Analysis Presentation.pptx`
  - Recorded presentation: `Border Crossing Analysis Video.mp4`

### Key Files
- `Border_Crossing_Entry_Data.csv`: Cleaned dataset used for analysis
- `Border_Crossing_Analysis.twb`: Tableau workbook with all visualizations
- `Border Crossing Entry Data Analysis.docx`: Comprehensive analysis report
- `Border Crossing Analysis Presentation.pptx`: Presentation slides
- `Border Crossing Analysis Video.mp4`: Recorded presentation video

## 13. Git Repository
All files are organized and version-controlled using Git. The complete repository is available for viewing and cloning via GitHub.
