# Code and data used for Cheung et al.

This repository contains the data, code, and documentation for the study: **“Racialized Economic Concentration Predicts Storm-Related Injuries and Deaths in the United States, 2005–2022”**

## Overview

This study investigates whether counties with higher ICE values, reflecting a greater concentration of high-income non-Hispanic White households relative to low-income Black households, experience lower rates of storm-related injuries and deaths.

By linking county-level ICE measures with NOAA’s Storm Events Database, we evaluate whether racialized economic concentration is associated with vulnerability to storm-attributed health harms, independent of population size.

This investigation is situated within a socioecological framework of public health. Racialized economic concentration reflects the spatial organization of advantage and disadvantage across populations and does not operate in isolation. It is shaped by and interacts with systems of housing, infrastructure, healthcare access, and emergency preparedness. These structural conditions may influence patterns of exposure, susceptibility, and recovery in the context of climate-related hazards.

By adopting this systems-level perspective, the analysis focuses on how structurally embedded inequalities contribute to differential vulnerability to storm-related injuries and deaths.

# Data Sources
## 1. Storm Events Data (2005–2022)
Source: National Oceanic and Atmospheric Administration (NOAA) Storm Events Database

Event Types Included: Hurricanes (Typhoons), Tropical Storms, Storm Surge/Tide, Coastal Floods, Flash Floods, High Winds, and Tornadoes.

Variables Used: Event type, county (FIPS), year, direct and indirect injuries, direct and indirect deaths.

## 2. Index of Concentration at the Extremes (ICE)
Source: IPUMS Contextual Determinants of Health Dataset

Metric: ICE for race-income (non-Hispanic White high-income vs. Black low-income households)

Time Frame: Overlapping 5-year ACS windows (e.g., 2005–2009, 2006–2010...)

Assignment: Each storm event is matched to the ICE window centered around its event year.

## 3. County-Level Population Data
Source: American Community Survey (ACS)

Use: Offset term in count models and calculation of rates.

# Software & Reproducibility
Language: R (version 4.5.0)

All code is reproducible and documented with comments. Scripts are intended to be run sequentially.

**Please contact Jason Cheung (jasoncheung@uchicago.edu) with any questions about this code.**
