# NCAA Athletic Department Expenses and Revenues
### Table of contents
- [Introduction](#problem-introduction)
- [Skills](#skills-overview)
- [Data Visualization](#data-visualization)
---
## Problem Introduction
![image](https://github.com/chile2706/PowerBI/assets/147631781/821162f6-1e88-466e-ae20-4f71d29efcdd)

![image](https://github.com/chile2706/PowerBI/assets/147631781/c5874005-8493-4192-95f5-c44bad6a0d1c)

![image](https://github.com/chile2706/PowerBI/assets/147631781/05e11aff-d94f-47e1-b226-7555a1f6f981)



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

![image](https://github.com/chile2706/PowerBI/assets/147631781/22d54cb6-9edc-4f78-9d16-4295b9fb075c)

``` DAX
Selected Measure = SWITCH(values('Measures Table'[Measures]), "Total Profits", sum(finances_fact[Total Profits]), "Total Revenues",sum(finances_fact[Total Revenues]), "Total Expenses", sum(finances_fact[Total Expenses]), sum(finances_fact[Total Revenues]))
```

Over Year

![image](https://github.com/chile2706/PowerBI/assets/147631781/045a0d59-2001-40ba-b243-19a31487e65f)
![image](https://github.com/chile2706/PowerBI/assets/147631781/09c517fc-127d-4fbf-b02a-af03d501dcac)


By Conference

![image](https://github.com/chile2706/PowerBI/assets/147631781/5a5dea2b-88f1-4f2f-8775-c5d1aa7f6342)
![image](https://github.com/chile2706/PowerBI/assets/147631781/c23569ce-7dfb-473d-9276-d2ff3d59c81b)


### Slicer

![image](https://github.com/chile2706/PowerBI/assets/147631781/c223b9fc-a6da-458f-9a69-f15787675e39)
![image](https://github.com/chile2706/PowerBI/assets/147631781/4d921f4f-b196-48ec-97a8-548859775b30)







