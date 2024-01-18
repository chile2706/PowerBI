# Maximum ice coverage over time for the US Great Lakes
### Table of contents
- [Introduction](#problem-introduction)
- [Skills](#skills-applied)
- [Data Transformation](#data-transformation)
- [Data Visualization](#data-visualization)
---
## Problem Introduction
![Page 1](https://github.com/chile2706/PowerBI/assets/147631781/60e6a7d3-5b39-45ec-96fd-411cb18218b6)
![Page 2](https://github.com/chile2706/PowerBI/assets/147631781/20359b59-61a0-466e-a7f8-c0d476d859a1)



* This dashboard was based on [Power Bi 2021 Week 7 Challenge by Workout Wednesday](https://workout-wednesday.com/pbi-2021-w07/)
#### Data set:
* `maximum ice coverage` data from NOAA’s Great Lakes Environmental Research Laboratory. A lake can have ice coverage ranging from 0 (no ice) to 100 (frozen over). [Link](https://data.world/dataveld/wow2021week07)
![image](https://github.com/chile2706/PowerBI/assets/147631781/6e1ac355-4084-4184-85b2-73bb81365bac)

---
## Skills Overview
* `Button`
* `Matrix conditional formatting`: display different ranges of Maximum Ice coverage over time for the US Great Lakes.
* `Forcasting`: forcast the Average Ice coverage out to 2030
* `Anomaly Detection`: determine the anomalies in Average Ice coverage by Year

---
## Data Transformation
* `Unpivot`: change the individual lake columns into rows
* `Year Format to use Forcasting`
![image](https://github.com/chile2706/PowerBI/assets/147631781/a7c9966b-b871-4680-8f42-fe713a0554f4)
---
## Data Visualization
* [Page 1: Conditional Formating](#page-1)
* [Page 2: Forcasting and Anomaly Detection](#page-2)
### Page 1
- [Slicer: Year Range](#[slicer]-year-range)
- [Line chart: Average Coverage by Year](#[line-chart]-average-coverage-by-year)
- [Bar chart: Maximum Historical Coverage](#[bar-chart]-maximum-historical-coverage)
- [Matrix: Maximum Coverage by Lake](#[matrix]-maximum-coverage-by-lake)
- [Button: navigate to Page 2](#[button]-navigate-to-page-2)
- [Insights](#insights)
![Page 1](https://github.com/chile2706/PowerBI/assets/147631781/60e6a7d3-5b39-45ec-96fd-411cb18218b6)

#### [Slicer] Year Range
(snapshot)

#### [Line chart] Average Coverage by Year
- add Line chart element, add Year field to x-axis, add Max coverage to y-axis, set coverage to avg
- fit trend line
(snapshot)

#### [Bar chart] Maximum Historical Coverage
- choose Max
- add label inside bars

#### [Matrix] Maximum Coverage by Lake
- Add:
- Exclude `All lakes`
- Removing row total and column total
- exclude `All lakes` for every visuals on the page
- conditional formating:
    * Background color: Build a set of conditional formatting Rules to Use five different colors for ice coverage (<25, <50, <75, <100, 100)
    * Build and apply Rules so that the contrast between your background colors and white or black font color passes the accessibility test for WCAG AA at https://contrastchecker.com
    * Add a star next to any value where the maximum ice coverage is 100%

#### [Button] navigate to Page 2
(snapshot)

### Page 2
- [Maxtrix: Min and Max Ice coverage of each lake of all time]()
- [Forcasting Line Chart: Average Coverage by Year]()
- [Anomalies Line Chart: Average Coverage by Year]()



