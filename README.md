# Retirement-Project
A Comprehensive Overview of Retirement Ages Worldwide

<img src="https://github.com/Khalih-01/Retirement-Project/blob/main/images/Intro.webp"/>

## Introduction
This project delves into the intricacies of retirement ages worldwide, seeking to uncover patterns and trends that define this crucial life transition. By examining data from various countries, we aim to comprehend the existing retirement age landscape.

#### Tableau Concepts Applied:
- Calculated Fields, Parameters, Filters, Table Calculations, Level of Detail (LOD) Expressions, Formatting, Dashboard Actions.

## Problem Statement
- How do retirement ages of each country compare to OECD average
- Which country has the earliest retirement age 
- Which country has the earliest retirement age for male and female

## Skills Demonstrated
Design Thinking, Data Processing, Descriptive Statistics

## Data Sourcing 
The Organisation for Economic Co-operation and Development (OECD) is an intergovernmental organisation with 38 member countries, Data was sourced from OECD ([Download Here](https://data.world/makeovermonday/2023w16)), I then imported it into Tableau for Transformation, Analysis and Visualization

The dataset contains 1 Sheet with 1175 rows and 7 columns

## Data Transformation
I excluded values in the country column that weren’t countries and edited aliases to properly represent each country. 
After a thorough examination of all columns, they were confirmed to be valid, free from empty cells, and devoid of errors. However, it was highly important I transformed the year column because the intervals were not uniform. This involved creating a set with consistent 10-year intervals, a deliberate choice that resulted in a more standardized and analytically useful representation of the temporal data.

#### Calculated Fields & Parameters

A calculated field is a field that uses existing database fields and applies additional logic, Calculated fields allow you to create new data from data that already exists in your data source. 

Calculated Field  | Image  | Description
:--------:|:---------------------------: |:----
OECD Average| <img src="https://github.com/Khalih-01/Retirement-Project/blob/main/images/OECD%20Average.png" width="5000"/>| For each Year and Gender, This expression calculates the average age for countries in the OECD, taking into account only the rows where the country is 'OECD - Average'. The fixed level of detail (LOD) Expression ensures that this calculation is done independently for each year and gender.

Parameters serve as dynamic inputs that enable users to interactively modify aspects of a visualization, In order for a parameter to work, they need to be tied to a calculated field. 

The following parameters will enable the user to interactively change the Gender,Year and Country aspect of the visualization.
Gender | Year | Country
:-------:|:-----:|:-------:
<img src="https://github.com/Khalih-01/Retirement-Project/blob/main/images/Gender%20Parameter.png"  width="750"/>| <img src="https://github.com/Khalih-01/Retirement-Project/blob/main/images/Year%20Parameter.png" width="800"/> | <img src="https://github.com/Khalih-01/Retirement-Project/blob/main/images/Country%20Parameter.png" width="750"/>
<img src="https://github.com/Khalih-01/Retirement-Project/blob/main/images/Pick%20Gender.png"  width="750"/>| <img src="https://github.com/Khalih-01/Retirement-Project/blob/main/images/Pick%20year.png" width="800"/> | <img src="https://github.com/Khalih-01/Retirement-Project/blob/main/images/Selected%20Country.png" width="750"/>


## Analysis & Visualization

<img src="https://github.com/Khalih-01/Retirement-Project/blob/main/images/Retirement%20Ages.png"/>

This visualization offers a global perspective on early retirement, The tooltip dynamically displays a comparative analysis when hovering over each country. Notably, this comparative analysis compares each countries average retirement ages to the OECD average. 
Clicking on a specific country in the tile chart triggers the presentation of a detailed bar chart. Notably, this bar chart compares the average retirement ages of men and women within the selected country.

https://github.com/Khalih-01/Retirement-Project/assets/114422925/1f1cec7a-a388-4c7b-898c-d2884b92d956

The user is granted significant control over the visualization. Through interactive elements (Parameters), one can modify the Gender and Year, tailoring the analysis to specific preferences. 
Leveraging the power of table calculations, the tile chart was built, and the incorporation of dashboard actions transformed it into a parameter. This parameter allows users to dictate which country's bar chart is displayed, ensuring a personalized and user-driven exploration of retirement trends worldwide.

Interact with visualization ([Here](https://public.tableau.com/views/RetirementAgesAroundtheWorld_17010424073140/RetirementAges?:language=en-GB&:display_count=n&:origin=viz_share_link))

#### Key Insights
- South Africa had the earliest Retirement Age in 2020 with 58.20 years.
- Indonesia had the latest Retirement Age in 2020 with 68.95 years.
- Saudi Arabia had the earliest Retirement Age for Men in 2020 with 58.90 years.
- Indonesia had the latest Retirement Age for Men in 2020 with 68.70 years.
- South Africa had the earliest Retirement Age for women in 2020 with 56.00 years.
- Indonesia had the latest Retirement Age for women in 2020 with 69.20 years.









