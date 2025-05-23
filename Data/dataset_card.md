## Ixodes pacificus Questing Behavior Dataset Card

Dataset title: Ixodes pacificus Questing Behavior

Dataset curator: Timara Vereen, MS graduate student, Swei Lab, Department of Biology, San Francisco State University (SFSU)

Dataset version: 1.0, 4.5.25

Dataset citation and DOI: Data statement author: Timara Vereen, MS graduate student, Swei Lab, Department of Biology, San Francisco State University

Data statement citation: authors, date, title, version, institution, and URL or DOI.

## Languages

English

## Dataset Overview

Title: Ixodes pacificus Questing Behavior Dataset

Description: This dataset contains observations of questing behavior in Ixodes pacificus nymphal ticks, focusing on vertical movement and activity levels. The data explores the influence of geographic origin on questing behavior across different locations in California.

Source: Data collected from controlled laboratory trials and field sampling in California.

Collection Process: Each tick was observed over a 5-minute trial, with movement recorded at 30-second intervals. The dataset includes multiple trials per tick and considers factors such as engorgement level and population origin.
Bioinformatics: Raw movement and position data were used to calculate activity metrics, and data were organized into a tidy structure using R.

## Data Instances

This dataset can be used to analyze tick questing behavior in relation to geography and environmental conditions. It may inform public health strategies for vector-borne disease prevention.
                  
| Population          | Room | Engorgement | Tick_ID     | Trial | X_sum | Y_sum | Z_sum | horizontal_dist | vertical_gross_dist | max_vert | total_dist | movement_count | percent_activity | vertical_or_no |
|---------------------|------|-------------|-------------|-------|--------|--------|--------|------------------|----------------------|----------|-------------|-----------------|------------------|----------------|
| Northern California | U    | 1           | 24FL_0.001  | 1     | 4      | 2      | 0      | 2.000000         | 0.0000               | 0        | 2.00000     | 2               | 18.181818        | 0              |


## Dataset Details
| Column Name               | Description                                                     |
|---------------------------|---------------------------------------------------------------  |
| Tick_ID                   | Unique identifier for each tick                                 |
| Trial_Number              | Trial iteration number                                          |
| Time                      | Time interval during the trial (every 30 seconds)               |
| Vertical_or_no            | Whether tick moved vertically (1 = yes, 0 = no)                 |
| Movement_Count            | Number of observed movements during the trial                   |
| Percent_Activity          | Percentage of time the tick was active during the trial         |
| Population                | Geographic origin of the tick (e.g., Northern California)       |
| Engorgement_Level         | Blood-meal feeding state; ranked level of engorgement (1 to 3)  |
| Vertical_distance_gross   | Total vertical movement documented during the trial             |
| X_sum                     | Total x-axis movements documented during the trial              |
| Y_sum                     | Total y-axis movements documented during the trial              |
| Z_sum                     | Total z-axis movements documented during the trial              |
| Horizontal_distance       | Distance traveled on the x & z planes during the trial          |
| Room                      | Location where experiment was conducted:U-Upstairs; D-Downstairs| 
## Rationale

This dataset was created to evaluate variation in tick behavior that could influence host encounters and pathogen transmission. Understanding behavioral differences by population origin and geographical differences helps inform ecological and public health research related to Lyme disease dynamics in California.

## Annotations

Data points and tick movement were documented every 30 seconds over the course of 3, 5-minute trials.

## Annotation Process

Raw tick movement was determined based on positional changes between time intervals.
All variables were calculated using formulas and programs in Excel and/or R script.

## Annotator

Data from behavioral experimentations and field samples were conducted by Timara Vereen, a current master's student in Dr. Andrea Swei's Lab at SFSU.

## Personal and Sensitive Information

This dataset contains no personal information.

## Social Impact of Dataset

This dataset contributes to ecological understanding of tick behavior and Lyme disease transmission risk.

## Discussion of Biases

Trials were conducted in a lab setting and doesn't mimic a natural host-seeking behavior.

There were high reports of inactive ticks which skewed activity measures.

Sampling locations were limited within this study and may not reflect the full geographic range and their influence.

## Other Limitations

Nymphal ticks were tested during this project, however, behavior may differ in larvae or adults tick life stages.


## Licensing Information
Licensing through the Creative Commons Attribution 4.0 (CC BY 4.0). Feel free to use this data for analysis and reference; please give the appropriate credit :)

## Contributions

Funding for this research was supported by San Francisco State University Student Enrichment Opportunities (SEO) and National Institutes of Health Bridge to the Doctorate Program (T32-GM142515)  Special thanks to faculty and staff at SFSU, my undergraduate mentee, Kathleen Hill-Oubre, and my fellow Swei Lab peers.

