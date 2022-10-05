# [View Presentation Here!](</presentation_slides.pdf>)

# Exploring the Relation Between Yankees Home Games and MTA Subway Stations

*Matteo Fortier*

## Abstract

The goal of this project was to undertake an exploratory data analysis on the relationship between Yankees Home Games at Yankees Stadium and the foot traffic of MTA Subway stations. The purpose of the analysis was to provide solutions for maintaining safe subway travel as events begin to return to pre-covid normalities. MTA turnstile data, combined with the Yankees 2019 schedule data obtain from baseball-reference allowed for the analysis of their relationship. The project then visualised the results of the analysis using matplotlib and seaborn.  

## Design

The current news of NYC beginning to ease covid restrictions inspired the idea for this project. The current trend is that events are starting to return to regular frequencies and capacities. However, the pandemic is not entirely over yet, and thus certain groups may be concerned about increased crowd sizes, especially in essential areas such as a subway station. Thus it is essential to analyse how events like baseball games affect surrounding stations and possible solutions for those affected by crowds. 

## Data

The project used two data sets. The primary dataset was the MTA turnstile dataset, used to obtain the foot traffic of MTA stations. Each entry represented the cumulative entries a single turnstile had recorded at a particular point in time. The second dataset was the 2019 season schedule for the Yankees provided by baseball-reference, providing home game dates and the attributes associated with those games. The project joined the two datasets, allowing for the relationship between home games (and their data) and the foot traffic of MTA stations to be analysed. The project focused on the 2019 year for both datasets as it provided a more accurate representation of regular commuting and events. 

## Algorithms

Exploratory data analysis included steps of cleaning, exploring, aggregating and visualising. Cleaning involved using SQL and Pandas to handle incorrect or missing values, selecting specific rows or columns, and the creation/manipulation of rows to make exploration more effective and accurate. Exploration and aggregation involved using pandas to manipulate data, allowing for relevant information to be processed and analyse. 

## Tools

Raw datasets were ingested into a jupyter notebook using an SQLite database via the Quick Setup provided. Querying from the SQLite database into Python involved using SQLAlchemy and SQLite queries.
Database cleaning and aggregation utilised SQLAlchemy and Pandas.
Exploratory data analysis mainly involved using Pandas, matplotlib and seaborn for initial visualisations. Finally, the project visualised findings using the matplotlib library and the seaborn library.

## Communication

The project used google slides for the presentation and the previously mentioned visualisation libraries for the visuals. 
