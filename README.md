# Age_DOE_buildings

It seems that more recent schools are more likely to be rated higher. I'm refining this analysis by looking at:

1) The exact relationship between building age and accessibility (correlation, regression) 

1) where schools built after the Americans with Disabilities Act was passed are; a lot more in Queens than other boroughs

2) what the age distribution of NYC schools is and how they correspond with the tenures of school building superintendents in the last century
___

DATA SOURCES FOR ANALYSIS 1:

2017-2018 School_Locations.csv (https://data.cityofnewyork.us/Education/2017-2018-School-Locations/p6h4-mpyy), because I want to combine DOE Building Codes with Borough Block and Lot codes

School-NYC-Accessibility-geolocated.csv (https://github.com/kpananjady/Accessibility-NYC-Schools/blob/master/School-NYC-Accessibility-geolocated.csv), because I'm only interested in the codes that have been rated already by the DOE

pluto_20v1.csv (https://www1.nyc.gov/site/planning/data-maps/open-data/dwn-pluto-mappluto.page), to get the year buildings were built and whether or not they're landmarks/located in historic districts
___

ANALYSIS 1: GETTING THE DATA READY
In the file Merges and Wrangling.ipynb (https://github.com/kpananjady/Age_DOE_buildings/blob/master/Merges%20and%20wrangling.ipynb), I get all my data ready so I can access the year built for 95 percent of the school buildings in my rated dataset. 

I start by combining school locations and accessibility ratings on DOE building codes, and then combine the resulting file on the Pluto database on borough, block and lot codes. This gives me the year built for most of the rated building in the DOE dataset.

I then try to get year built for every single school location — whether or not they've been rated so far. I plot the distribution of construction years for all buildings, and then another histogram for all

RESULT: years_built_school.csv (https://github.com/kpananjady/Age_DOE_buildings/blob/master/year_built_school.csv) for the years when rated schools were built; all_schools_years.csv (https://github.com/kpananjady/Age_DOE_buildings/blob/master/all_schools_years.csv) for the years when all schools were built
___
DATA SOURCES FOR ANALYSIS 2:

years_built_school.csv (https://github.com/kpananjady/Age_DOE_buildings/blob/master/year_built_school.csv) for the years when rated schools were built, generated above
___
ANALYSIS 2: RELATIONSHIP BETWEEN BUILDING AGE AND ACCESSIBILITY

In Age Analysis.ipynb (https://github.com/kpananjady/Age_DOE_buildings/blob/master/Age%20Analysis.ipynb), I explore the relationship between building age and accessibility rating mathematically. In the QJIS files, I map out the patterns I see, the results of which you can see in the screenshots. 

Screenshot 1( https://github.com/kpananjady/Age_DOE_buildings/blob/master/Screen%20Shot%202020-03-29%20at%206.33.10%20PM.png) shows all the buildings rated 10; Screenshot 2 (https://github.com/kpananjady/Age_DOE_buildings/blob/master/Screen%20Shot%202020-03-29%20at%206.33.22%20PM.png) overlays schools built between 1984-2017. 

___

For the first part of this accessibility analysis, please see https://github.com/kpananjady/Accessibility-NYC-Schools. 
