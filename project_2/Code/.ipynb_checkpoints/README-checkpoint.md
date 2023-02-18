# Project 1: Exploring climate data of Singapore

### Overview
This project looks at the rainfall and tidal data to find recommendations for National Outdoor Adventure Singapore 
(NOAS). NOAS is an outdoor adventure provider that designs and conducts programme for Institure of Higher Learning (IHL)
students in Singapore. One of the key programme is the 9-days, Singapore Youth Outdoor (SYO) programme that is held
annually for all IHL students. The programme objectives is to build social cohesion and resilience amongst the IHL
students.SYO has been well-received and it is in its 5th year running. However, lately there were multiple feedback on
one of the programme's activities i.e. Kayaking.

---

### Problem Statement
SYO students feedback that the kayaking expedition route is too short and easy. They are looking for a longer expedition
route that is challenging and stretches them physically, emotionally and mentally. 
NOAS has been tasked to looked into extending the expedition route. However, before the new route can be implemented, a
trial needs to conducted and assessed by NOAS Safety Committee Members (SCM). Hence NOAS is looking for the ideal month
to conduct the new expedition trial route. Key considerating factors are:
> 1. low to minimal rainfall for the month; 
> 2. longer duration of sunshine hours with reasonable humidity level; and
> 3.  favorable tidal conditions.

The assumption is that with heavy rainfall comes thunderstorms which will significantly impact the success of the trial.
Hence mitigating those factors will greatly increase the chance of success because students can paddle confidently and
safely. 

---

### Datasets

|Feature|Type|Dataset|Description|
|---|---|---|---|
|total_rainfall_by_month|float|rainfall-monthly-total|Total rainfall in mm| 
|rainy_days_by_month|float|rainfall-monhtly-number-of-rain-days|days that have recorded rainfall at 2mm, are considered
rainy days|
|humidity_by_month|float|relative-humidity-monthly-mean|average humidity for the month|
|sunshine_hours_by_month|float|sunshine-duration-monthly-mean|average sunshine hours for the month|
|tide_table|float|2022_tidetable|tidal conditions for the month|

---

### Brief Summary of Analysis
From the analysis, Jan 2022 seem to be the ideal month to conduct the new expedition trial route due to the following
reasons:
> 1. minimal rainfall;
> 2. longer duration of sunshine hours;
> 3. reasonable humidity level; and
> 4. favorable tide conditions.

---

### Visualisations Used
The following visualisations were used:
> 1. scatter plot to measure the distribution of rainfall, humidity and sunshine hours;
> 2. line plot to measure the distribution of the tidal height across the months and the tidal difference; and
> 3. histograms(pairplot) and heatmap to measure the correlations between the features
All of your projects will comprise of a written technical report and a presentation. As we continue in the course, your technical report will grow in complexity, but for this initial project it will comprise:

---

### Conclusions and Recommendations
In summary, NOAS recommends to SCM to conduct the kayaking expedition trial route from Pulau Ubin to East Coast campus
at an estimated distance of 33km during Jan 2022. It is projected to be a success considering Jan has the lowest
rainfall and the longest duration of sunshine hours including favorable tidal conditions.
