# global-water-velocity-analysis

- Global Water Access: 20-Year Velocity & Trend Analysis (2000-2020)

1, Project Overview

This project investigates the "speed of progress" in global water sanitation. Using the WHO/UNICEF Joint Monitoring Programme (JMP) dataset, I developed a model to calculate the Annual Rate of Change (ARC) for over 200 countries across two decades. The goal was to identify which global regions are effectively closing the infrastructure gap.

2, Technical Workflow & Data Engineering 
- Longitudinal Data Alignment: Sorted and structured a 3,000+ row dataset by country and year to ensure chronological integrity.
- Region Mapping: Integrated disparate datasets using VLOOKUP to categorize countries into seven global geographic regions.
- Time-Series Logic (y_diff): Engineered a custom logic column to handle irregular reporting intervals, ensuring the Annual Rate of Change was normalized regardless of the gap between data points.
- Annual Rate of Change (ARC) Modeling: Developed formulas to calculate the yearly percentage point improvement for National, Rural, and Urban sectors :Formula: $ARC = \frac{Water Access_{Year 2} - Water Access_{Year 1}}{Year_{2} - Year_{1}}$
