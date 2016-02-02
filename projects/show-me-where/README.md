# Show Me Where project

A **project showing me where things** are.

### another headline for fun


# About the dataset

The Palo Alto Police Department has posted a spreadsheet of reported incidents from up to 6 months ago. The dataset contains roughly 6,000 records and its fields include geolocations for approximate addresses of the incidents, as well as the disposition of the report.


## Basic facts about the dataset

- The source of the data: [City of Palo Alto, Open Data Portal, Police Department](http://data.cityofpaloalto.org/home)
- The data's landing page: [Crime Reports](http://data.cityofpaloalto.org/dataviews/95541/crime-reports/)
- Direct link to the data: [http://data.cityofpaloalto.org/rest/datastreams/107246/data.csv](http://data.cityofpaloalto.org/rest/datastreams/107246/data.csv)
- The data format: CSV
- Number of rows: 6,658

## Description of data fields

#### incident_datetime 

A datetime value, in this format: `"2015-06-03T04:45:00Z"`


#### description 

Contains a __text string__ that seems to be a standardized category for the reported incident, e.g. `"THEFT PETTY/MISC (488M)"`, `"THEFT GRAND/BIKE/BIKE PARTS (487B)"`

#### disposition

Contains a __text string__ of the status of the report, such as whether someone was arrested or cited, e.g. `"INACTIVE"`, `"MISD. CITATION"`



#### address

Contains a __text string__ of the street address of the incident location. The location is often described as being an intersection, e.g. `"EL CAMINO REAL & QUARRY RD"`, or a block, e.g. `"600 Block SAN ANTONIO AV"`


#### city  

Contains a __text string__ representing the city name of the incident location, e.g. `"Palo Alto"`


#### zipcode 

Contains a __text string__ representing the 5-digit ZIP code of the incident location, e.g. `"94043"`

#### latitude

Contains a __float__ that represents the latitude coordinate of the incident location.

#### longitude

Contains a __float__ that represents longitude coordinate of the incident location.

## Anticipated data wrangling

I will probably filter the dataset to include burglary-type crimes, such as car/home burglaries, and thefts of bikes and vehicles.


