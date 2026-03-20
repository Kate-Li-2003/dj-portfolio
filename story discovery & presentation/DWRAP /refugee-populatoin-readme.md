# Refugees by country of asylum - Data package

This data package contains the data that powers the chart ["Refugees by country of asylum"](https://ourworldindata.org/grapher/refugee-population-by-country-or-territory-of-asylum?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on January 12, 2026.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The final column is the data column, which is the time series that powers the chart. If the CSV data is downloaded using the "full data" option, then the column corresponds to the time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data column is transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

## Detailed information about the data


## Refugees by country of asylum
[People](#dod:refugee) who fled their country of origin because of serious threats against which the authorities of their home country cannot or will not protect them. This includes all refugees who live in this country, not just those who arrived that year.
Last updated: July 3, 2025  
Next update: July 2026  
Date range: 1951–2024  
Unit: people  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
UNHCR (2025) – with major processing by Our World in Data

#### Full citation
UNHCR (2025) – with major processing by Our World in Data. “Refugees by country of asylum” [dataset]. UNHCR, “Refugee Population Statistics Database Annual statistics for 2024” [original data].
Source: UNHCR (2025) – with major processing by Our World In Data

### What you should know about this data
* A refugee is a person in need of international protection, who had to flee their home country because of serious threats against which the authorities of their home country cannot or will not protect them.

### How is this data described by its producer - UNHCR (2025)?
Refugees include individuals recognized under the 1951 Convention relating to the Status of Refugees, its 1967 Protocol, the 1969 Organization of African Unity (OAU) Convention Governing the Specific Aspects of Refugee Problems in Africa, the refugee definition contained in the 1984 Cartagena Declaration on Refugees as incorporated into national laws, those recognized in accordance with the UNHCR Statute, individuals granted complementary forms of protection, and those enjoying temporary protection.

The refugee population also includes people in refugee-like situations.

### Source

#### UNHCR – Refugee Population Statistics Database
Retrieved on: 2025-07-03  
Retrieved from: https://www.unhcr.org/refugee-statistics/download/?v2url=e7088f  

#### Notes on our processing step for this indicator
- The United Nations High Commissioner for Refugees (UNHCR) collects data on refugee populations for each country of origin and country of asylum separately. To calculate the total number of refugees living in a country, we sum up the data from all origin countries. To calculate the total number of refugees from a country, we sum up the data from all asylum countries.
- To calculate the number of refugees per 1,000 or 100,000 people in a country, we divide the number of refugees by the total population of the country (for the same year) and multiply by the factor. The population estimates come from a long-run dataset [maintained by Our World in Data](https://ourworldindata.org/population-sources).
- We remove refugee populations where the country of origin and country of asylum are the same, as refugees are defined as people who have fled their country and crossed an international border. We also remove asylum seekers where the country of origin and country of asylum are the same.
- We remove data for China after 2020 due to a large data discontinuity.


    