# Income per GDP and Life Expectancy
### Table of contents
- [Introduction](#problem-introduction)
- [Skills](#skills-overview)
- [Data Visualization](#data-visualization)
---
## Problem Introduction
![image](https://github.com/chile2706/PowerBI/assets/147631781/6c0bd517-03f3-4200-b2bd-26c79ce5f0fd)

![image](https://github.com/chile2706/PowerBI/assets/147631781/626d4eda-0362-49fa-8d72-180b97295f5b)

![image](https://github.com/chile2706/PowerBI/assets/147631781/7ab398f2-b89f-4b69-9739-806f2fe3396b)



* This dashboard was based on [Power Bi 2021 Week 13 Challenge by Workout Wednesday](https://workout-wednesday.com/pbi-2021-w13/)

#### Data set:
This report is made of from 4 tables: `data geography`, `income per person`, `life expectancy years`, `population total` ([Link](https://data.world/missdataviz/wow2021-w11))

![image](https://github.com/chile2706/PowerBI/assets/147631781/8c4e10d9-89f2-4d06-879e-341831120200)

![image](https://github.com/chile2706/PowerBI/assets/147631781/e1df3744-8563-4832-bc83-aa4a5f692067)

![image](https://github.com/chile2706/PowerBI/assets/147631781/254705f5-5881-4cc9-9ba8-494fd18480bb)

![image](https://github.com/chile2706/PowerBI/assets/147631781/866512e5-2ff9-4fd5-b484-370621fef942)

---
## Skills Overview
* `Bubble Chart`:
  - shows life expectancy by average income over time
  - `color` of each bubble represent its Region
  - `size` of each bubble represents Population size
* `Custom Overlay`: gives additional details to end-users about the data included in the report
* `Button`: allow users to display the custom overlay

---
## Data Transformation
* `Unpivot`:
- create a new table by unpivoting `year` column

![image](https://github.com/chile2706/PowerBI/assets/147631781/b84ddcf7-f1dc-4e55-8294-276706e90364)

- create a relationship between new table with other tables (so that we can have year axis for our bubble chart)
![image](https://github.com/chile2706/PowerBI/assets/147631781/d2bbcbdf-8c81-4306-a764-b09dcb64035c)

---
## Data Visualization
* [Bubble Chart](#bubble-chart)
* [Custom Overlay](#custom-overlay)
### Bubble Chart

<img width=150 src="https://github.com/chile2706/PowerBI/assets/147631781/f5027cd6-eec8-4018-a966-476cb9458586">
<img width=800 src="https://github.com/chile2706/PowerBI/assets/147631781/6c0bd517-03f3-4200-b2bd-26c79ce5f0fd">




### Custom Overlay
- customize overlay by Powerpoint and then add it as a background to a new page
  
![image](https://github.com/chile2706/PowerBI/assets/147631781/ad3ec5e4-b399-40b6-b16e-080f72f4b8fe)


### Tooltip
- Create a Tooltip page with Card and Multi-row Card
  
![image](https://github.com/chile2706/PowerBI/assets/147631781/8f0d05ce-0e11-4559-802b-68053bb55807)


## Insights
**Are there any countries with an income over 50k that have an average life expectancy lower than 74?**


