# Electric_Vehicle_Population_Dashboard
## Overview
This project presents an interactive Excel dashboard created to analyse an Electric Vehicle Population dataset.

The dashboard provides insights into vehicle adoption, manufacturer popularity, electric vehicle types, electric range, model years, geographical distribution, and Clean Alternative Fuel Vehicle eligibility.

The project was completed using:

- Microsoft Excel
- Power Query
- PivotTables
- PivotCharts
- Slicers
- KPI cards

## Dashboard Preview
<a href= "">

Project Objectives
The purpose of this project was to answer the following questions:

How many electric vehicles are included in the dataset?
Which vehicle manufacturers have the highest number of registered vehicles?
Which vehicle models are the most common?
How are electric vehicles distributed across model years?
Which manufacturers have the highest average electric range?
How are vehicles distributed across CAFV eligibility categories?
What is the distribution of Battery Electric Vehicles and Plug-in Hybrid Electric Vehicles?
Which locations have the highest number of registered electric vehicles?
Dataset
The dataset contains information about registered electric vehicles, including location, vehicle characteristics, electric vehicle type, electric range, and CAFV eligibility.

Columns Used
Location Information
County
City
State
Postal Code
Full Location
Vehicle Information
Model Year
Make
Model
Model and Year
Electric Vehicle Information
Electric Vehicle Type
Clean Alternative Fuel Vehicle Eligibility
Electric Range
Valid Electric Range
Data Quality Issues
During the initial data review, I identified the following issues:

Blank and null values
Electric Range values equal to zero
Columns that were not relevant to the dashboard
Data types that required validation
Postal codes that needed to remain in text format
Long category names that required clear visual presentation
Data Cleaning Process
The dataset was cleaned and transformed using Power Query.

The main steps were:

Imported the dataset into Power Query.
Used data-profiling tools to inspect column quality and value distribution.
Checked and corrected column headers.
Checked and corrected data types.
Reviewed blank, null, error, and zero values.
Removed columns that were not required for the analysis.
Created a Full Location column.
Created a Model and Year column.
Created a Valid Electric Range column.
Converted Electric Range values equal to zero into null values in the validation column.
Created a reference query for dashboard development.
Loaded the base query as Connection Only.
Loaded the dashboard query as an Excel table.
Saved the final project as an XLSX workbook.
Calculated Columns
Full Location
The Full Location column combines City, County, State, and Postal Code.

[City] & ", " & [County] & ", " & [State] & " " & Text.From([Postal Code])
