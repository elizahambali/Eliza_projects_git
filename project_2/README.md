# Project 2: Predicting Singapore HDB Resale Price

### Overview
This project looks at the HDB Resale Data in Singapore. 
Prior to Singapore gaining independence in 1965, the Housing and Development Board (HDB) was already established to solve the housing needs of Singaporeans who were living in unhygienic conditions i.e. slums and squatter settlements. 

At that point only 9% of Singaporeans lived in government flats. 

The initial focus for HDB was to build affordable housing for low-income families while transforming Singapore's economic landscape to a newly-industrialised nation which meant a shift from rural and agricultural settlements to manufacturing. 
This meant land-scarce Singapore needed to prioritise its land usage for both residential and economic needs. 

HDB is now home to more than 80% of Singapore’s population, across 23 towns and 3 estates.

---

### Problem Statement
As of June 2019, according to the Department of Statistics – Population Trends 2019 publication, there are about 225,000 single Singapore Citizens within the age range of 35-39 years old who are eligible for public housing. 
Increasingly, people are putting marriage on hold as reported. Marriages and divorces are on the decline. Many prefer to remain single.

2 years later, an article in The Economist in 2021,  buttressed this trend revealing that more young single Singaporeans are moving out to live on their own, and are no longer happy living with their parents untill they are 35. 
Aside from the other demographics of families with young children, and elderly folks, policy makers in Singapore are considering reviewing the Single Singapore Citizen Scheme (or HDB Single Scheme)  introduced in October 1991 to allow single Singaporeans aged 35 and above to purchase HDB flats. 
With the cultural shift in living arrangement where the intergenerational families living under the same roof are upended, policy makers are trying to understand what features impact the resale price of HDB; in-turn influencing the buying choices of the following demographics with these general assumptions in the table below:

|SN|Dempgraphics|Assumptions|
|---|---|---|
|1|Families with young children|Prefer buying a house with considerable floor area to meet their needs i.e. 3 - 5 individuals in a flat, close to amenities such as schools, bus and/or mrt.
|2|Elderly and Singles |Prefer buying a house with considerable floor area for 1 - 2 individuals in a flat, close to amenities such as hawker centre, malls and bus and/or mrt.

While Singapore is land scarce, with an educated population who are marrying later, the initial focus of HDB to provide housing to just low income families bears some review. Balancing the needs between Singles aspiration to buy affordable HDBb before the age of 35, and factoring the increase in Elderly living on their own plus other national needs; policy makers have tasked the data science unit to provide an intepretative and predictive modelling of the housing price to further understand and inform the housing public policy.

---

### Datasets

|Feature|Type|Dataset|Description|
|---|---|---|---|
|town|object||HDB township where the flat is located, e.g. BUKIT MERAH|
|flat_type|object||type of the resale flat unit, e.g. 3 ROOM|
|flat_model|object||HDB model of the resale flat, e.g. Multi Generation|
|resale_price|float64||the property's sale price in Singapore dollars|
|Tranc_Year|int64||year of resale transaction|
|Tranc_Month|int64||month of resale transaction|
|lower|int64||median value of storey_range|
|upper|int64||median value of storey_range|
|mid|int64||median value of storey_range|
|floor_area_sqft|float64||floor area of the resale flat unit in square feet|
|hdb_age|int64||median value of storey_range|
|max_floor_lvl|int64||highest floor of the resale flat|
|commercial|bool||boolean value if resale flat has commercial units in the same block|
|market_hawker|bool||boolean value if resale flat has a market or hawker centre in the same block|
|multistorey_carpark|bool||boolean value if resale flat has a multistorey carpark in the same block|
|precinct_pavilion|bool||boolean value if resale flat has a pavilion in the same block|
|total_dwelling_units|int64||total number of residential dwelling units in the resale flat|
|1room_sold|int64||number of 1-room residential units in the resale flat|
|2room_sold|int64||number of 2-room residential units in the resale flat|
|3room_sold|int64||number of 3-room residential units in the resale flat|
|4room_sold|int64||number of 4-room residential units in the resale flat|
|5room_sold|int64||number of 5-room residential units in the resale flat|
|exec_sold|int64||number of executive type residential units in the resale flat block|
|multigen_sold|int64||number of multi-generational type residential units in the resale flat block|
|studio_apartment_sold|int64||number of studio apartment type residential units in the resale flat block|
|Mall_Nearest_Distance|float64||distance (in metres) to the nearest mall|
|Mall_Within_500m|float64||number of malls within 500 metres|
|Mall_Within_1km|float64||number of malls within 1 kilometre|
|Mall_Within_2km|float64||number of malls within 2 kilometres|
|Hawker_Nearest_Distance|float64||distance (in metres) to the nearest hawker centre|
|Hawker_Within_500m|float64||number of hawker centres within 500 metres|
|Hawker_Within_1km|float64||number of hawker centres within 1 kilometre|
|Hawker_Within_2km|float64||number of hawker centres within 2 kilometres|
|hawker_food_stalls|int64||number of hawker food stalls in the nearest hawker centre|
|hawker_market_stalls|int64||number of hawker and market stalls in the nearest hawker centre|
|mrt_nearest_distance|float64||distance (in metres) to the nearest MRT station|
|bus_interchange|float64||boolean value if the nearest MRT station is also a bus interchange|
|mrt_interchange|float64||boolean value if the nearest MRT station is a train interchange station|
|bus_stop_nearest_distance|float64||distance (in metres) to the nearest bus stop|

---

### Brief Summary of Analysis
From the analysis, the following factors that impact resale price are:
> 1. Location of Flat;
> 2. Age of Flat;
> 3. Storey Range of Flat; and
> 4. Floor Area of Flat.

---

### Models Used
The following Models were used:
> 1. Linear Regression;
> 2. Ridge CV; 
> 3. Lasso CY; and
> 4. Elastic Net

---

### Conclusions and Recommendations
While there are significant factors that impact HDB resale price, relying solely on this dataset to inform the housing policy is naive. There are other considerating factors such as the private housing and BTO data sets, population growth, economic growth, and other social policies that are required before considering lowering the age for Singles to buy an HDB before 35 years old.
