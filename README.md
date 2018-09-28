# Champaign County Police Use Cases

## Organization Name
- Champaign County Sheriff’s Office
- Rantoul Police Department
- Urbana Police Department
 
## Local Sponsor
Sanford Hess, IT Director of Urbana, responsible for the Area-wide Records Management Systems (ARMS) 

## Overview
These three police agencies in Champaign County share a common Records  Management System (called “ARMS”) that contains information on police activity.  Due to their use of a common system, the data has a consistent format - although some code values are unique to each jurisdiction for local ordinances.

## Problem Statement
Police records are commonly requested sets of data for analysis of both crime and police interactions with the public.  Police data can be useful for analysis on its own, or combined with other data about the population to gain insights.  For example, the United States Census Bureau has datasets by County and some by “Census block” https://www.census.gov/topics/population/data.html.  These police agencies are looking for creative uses of the data that could lead them into further analysis using more granular datasets.

## Evaluation criteria
- Insights on trends visible in existing data.
- Creative use of other datasets in combination with the data.
- Creatives ideas for further analysis that could be performed by the police agencies themselves.

## Data Details
| File Name | Description | Link |
| --------- | ----------- | ---- |
| [police_incidents.csv](https://www.dropbox.com/s/tw5878lg0n97r11/police-incidents.csv?dl=0) (DropBox link) | Police Incidents.  Each record is a specific “incident code” and some time/place information about the incident.  Incident codes can represent crimes, “Calls for Service”, or Administrative Codes that represent police actions.  Addresses are rounded to the block level for privacy, and for some types of events the addresses are removed completely to protect the victims. | https://data.illinois.gov/dataset/police-incidents |
| police_arrests.csv | Police Arrests.  Each record is an arrest charge against a person who has been taken to jail, or has been issued a citation in lieu of an arrest.  If a person has multiple charges, then each of them will be a record in the dataset - but they will have a common incident number.  Information about the arrestee is anonymized to show information such as age, race, home city, and sex - but no further details. | https://data.illinois.gov/dataset/police-arrests | 
| police_traffic_stops.csv | Police Traffic Stops.  Each record records the information about a driver who was stopped, as captured for the Illinois Department of Transportation (IDOT) Traffic Stop program.  In addition to the fields captured for IDOT, these records include the incident code recorded in the stop. Data goes back to 2012, when IDOT began using the current reporting layout. Wolfram One view of the data is here: https://datarepository.wolframcloud.com/resources/Urbana-Police-Stop-Sheets. | https://data.illinois.gov/dataset/traffic-stops |
| police_stop_sheets.csv | Police Stop Sheets.  Each record records the information about a person who was stopped and possibly frisked and/or searched, as captured for the Illinois Department of Transportation (IDOT) Stop Sheet program.    Data is presented since the Stop Sheet collection began in 2016.  Not all Stop Sheets displayed are submitted to the Illinois Department of Transportation (IDOT), so there is a field that indicates if the record is one that would be sent to the State. | https://data.illinois.gov/dataset/stop-sheets |
