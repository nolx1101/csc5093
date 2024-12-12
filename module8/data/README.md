# Data Folder

## Overview
This folder contains the dataset used for the **Border Crossing Analysis** project. The dataset has been pre-processed and cleaned to ensure accuracy and consistency in analysis and visualization.

## Files

### `Border_Crossing_Entry_Data.csv`
- **Description**: This dataset contains monthly records of border crossings at U.S.-Canada and U.S.-Mexico borders. It includes information on transportation modes, crossing volumes, and geographic locations (ports and borders).
- **Source**: Bureau of Transportation Statistics, Data.gov.
- **Format**: CSV file (`.csv`).

### Dataset Features
- **Port of Entry**: Specifies the border crossing location.
- **Border**: Indicates whether the crossing occurred at the U.S.-Canada or U.S.-Mexico border.
- **Measure**: Describes the type of crossing (e.g., trucks, buses, personal vehicles, pedestrians).
- **Value**: The number of crossings for each measure.
- **Date**: Monthly records for each crossing type.

### Data Cleaning
The following cleaning steps were applied to the raw dataset:
1. **Date Formatting**: Converted the `Date` column to a standard `MM-DD-YYYY` format for time-series analysis.
2. **Border Standardization**: Simplified entries in the `Border` column to `US-Canada` and `US-Mexico` for consistency.
3. **Missing Data**: Addressed gaps in crossing values by either aggregating data or excluding incomplete entries.

## Usage
This dataset is used in:
1. Tableau visualizations (`Border_Crossing_Analysis.twb`).
2. Exploratory and explanatory analysis documented in `Border Crossing Entry Data Analysis.docx`.

### Recommended Tools
- **Tableau**: For interactive visualizations and dashboard creation.
- **Excel**: For initial exploration and modifications if needed.
- **Python**: For advanced data preprocessing.

## Source Citation
- Bureau of Transportation Statistics. (2024). *Border Crossing Entry Data*. Retrieved from [https://catalog.data.gov/dataset/border-crossing-entry-data-683ae](https://catalog.data.gov/dataset/border-crossing-entry-data-683ae).
