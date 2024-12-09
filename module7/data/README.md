# Data Directory

## Overview
This folder contains the source data used for two projects in Tableau:
1. **Visual Resume**: The data is stored in the `Resume.xlsx` file, divided into multiple sheets.
2. **Border Crossing Analysis**: The data is stored in the `Border_Crossing_Entry_Data.xlsx` file, which includes U.S. border crossing entry data.

## Data Files

### 1. **Resume.xlsx**
- **Purpose**: Contains data for creating the visual resume in Tableau.
- **Data Sheets**:
  1. **Education Timeline**:
     - **Columns**: Institution, Degree, Start Year, End Year.
     - **Purpose**: Used for the Gantt chart to show educational milestones.
  2. **Skills**:
     - **Columns**: Skill Name, Proficiency (0-100%).
     - **Purpose**: Used for the bar chart to visualize skill proficiency levels.
  3. **Experience**:
     - **Columns**: Job Title, Company, Start Date, End Date, Location, Combined Details.
     - **Purpose**: Used for the map to display job locations and details.
  4. **Hobbies**:
     - **Columns**: Hobby, Time Spent (Years).
     - **Purpose**: Used for the bubble chart to represent hobbies and time spent.

### 2. **Border_Crossing_Entry_Data.xlsx**
- **Purpose**: Contains U.S. border crossing entry data used for analyzing and storytelling in the **Border Crossing Analysis** Tableau project.
- **Columns**:
  1. **Port Name**: Name of the border crossing port.
  2. **State**: U.S. state where the port is located.
  3. **Border**: Indicates U.S.-Mexico or U.S.-Canada border.
  4. **Date**: Month and year of the crossing data.
  5. **Measure**: Type of crossing (e.g., Trucks, Pedestrians, Personal Vehicles).
  6. **Value**: Number of crossings for the given measure.
- **Purpose**:
  - Analyzes trends in border crossings over time.
  - Provides insights into transportation modes, busiest ports, and regional differences.

## Key Files
- **Resume.xlsx**: Dataset for the Visual Resume project.
- **Border_Crossing_Entry_Data.xlsx**: Dataset for the Border Crossing Analysis project.
