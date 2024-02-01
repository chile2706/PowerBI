# NCAA Athletic Department Expenses and Revenues
### Table of contents
- [Introduction](#problem-introduction)
- [Skills](#skills-overview)
- [Data Visualization](#data-visualization)
---
## Problem Introduction
![image](https://github.com/chile2706/PowerBI/assets/147631781/ca22b460-d452-41e4-9693-1d592bf91331)
![image](https://github.com/chile2706/PowerBI/assets/147631781/7976dda4-608f-4111-ba3d-c22cef315985)
![image](https://github.com/chile2706/PowerBI/assets/147631781/1b2febe7-2913-46dc-8926-14ba529182bd)



* This dashboard was based on [Power Bi 2021 Week 8 Challenge by Workout Wednesday](https://workout-wednesday.com/pbi-2021-w08/)

#### Data set:
This report is made of from 3 tables: `finances_fact`, `school_dim`, `conference_dim`([Link](https://data.world/jbaucke/2021-w8-power-bi-wow-switching-metrics/workspace/file?filename=NCAA+Profit+and+Losses+Summarized.xlsx))

`conference_dim`

![image](https://github.com/chile2706/PowerBI/assets/147631781/b9733f74-07f5-4588-b84d-44811eaac92f)

`finances_fact`

![image](https://github.com/chile2706/PowerBI/assets/147631781/ae98a743-de52-4933-a0e5-b0de7fb36e15)

`school_dim`

![image](https://github.com/chile2706/PowerBI/assets/147631781/3ab711df-4ad2-4d05-9f87-5ee34de1d3bf)


---
## Skills Overview
Create a report view allows users to toggle between the metrics Total Revenues, Total Expenses, and Total Profits
  - create a `Measures Table` using `SWITCH()`function
  - create a `slicer` to allow users to toggle between the metrics
  - custom specific color for each metric

---
## Data Visualization
### Measures Table

``` DAX
Selected Measure = SWITCH(values('Measures Table'[Measures]), "Total Profits", sum(finances_fact[Total Profits]), "Total Revenues",sum(finances_fact[Total Revenues]), "Total Expenses", sum(finances_fact[Total Expenses]), sum(finances_fact[Total Revenues]))
```
![image](https://github.com/chile2706/PowerBI/assets/147631781/11a04684-01a8-49f7-89b7-7fb8e82bdf4c)

### Slicer
- List how you do it






