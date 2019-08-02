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
| police_arrests.csv | Arrests by the Urbana Police Department since 1988, with arrestee demographic data. Each record is an arrest charge against a person who has been taken to jail, or has been issued a citation in lieu of an arrest.  If a person has multiple charges, then each of them will be a record in the dataset - but they will have a common incident number.  Information about the arrestee is anonymized to show information such as age, race, home city, and sex - but no further details.  Wolfram One view of the data: https://datarepository.wolframcloud.com/resources/Urbana-Police-Arrests-Since-1988.  | https://data.illinois.gov/dataset/police-arrests | 
| police_incidents.csv.gz | Police Incidents since 1988..  Each record is a specific “incident code” and some time/place information about the incident.  Incident codes can represent crimes, “Calls for Service”, or Administrative Codes that represent police actions.  Addresses are rounded to the block level for privacy, and for some types of events the addresses are removed completely to protect the victims. | https://data.illinois.gov/dataset/police-incidents |
| idot_traffic_stops.csv | The information is the same data transmitted to the Illinois Department of Transportation (IDOT) with two additions: the "Motivation for Stop", and the offense codes recorded. Data goes back to 2012, when IDOT began using the current reporting layout. Wolfram One view of the data is here: https://datarepository.wolframcloud.com/resources/Urbana-Police-Traffic-Stops. | https://data.illinois.gov/dataset/traffic-stops |
| idot_stop_sheet.csv | Stop Sheet results from the City of Urbana, since the Stop Sheet collection began in 2016. Not all Stop Sheets are submitted to the Illinois Department of Transportation (IDOT), so there is a field that indicates if the record is one that would be sent to the State.  Example notebook from Wolfram: https://datarepository.wolframcloud.com/resources/Urbana-Police-Stop-Sheets. | https://data.illinois.gov/dataset/stop-sheets |
| nuisance_data.csv | Nuisance complaints reported on properties in Urbana, with the type of complaint, resolution, and fine amounts. For privacy, addresses are anonymized to the block level. Contains records from 2003.  | https://data.illinois.gov/dataset/urbana-nuisance-complaints |
