# About Dataset

This dataset can be accessed from my KAGGLE [datasets](https://www.kaggle.com/datasets/shilongzhuang/us-school-shootings-19702022) portfolio. 

## Collection Methodology
All data was downloaded from the K-12 School Shooting Database (K-12 SSDB), which comprehensively compiles documents when a gun is brandished, is fired, or a bullet hits school property for any reason, regardless of the number of victims, time of day, or day of week. Simple excel querying was then done to separate the multiple sheets in the downloaded file. If you are interested, it is highly advisable to go over their research methodology to understand how they conduct research and compile the data from multiple data sources

- Link to the Database: https://www.chds.us/ssdb/
- Research Methodology: https://www.chds.us/ssdb/methods/

## Content
The dataset is structured as a relational database (compilation of multiple sheets) referenced with a unique incident ID number that links to the corresponding INCIDENT, SHOOTER, VICTIM, and WEAPON files.

- INCIDENT: Incident ID number and the information related to the what, where, and when the shooting happened.
- SHOOTER: Incident ID number and details about the shooter. Multiple rows that have similar incident ID numbers indicate multiple shooters involved.
- VICTIM: Incident ID number and details about the victim. Multiple rows have the same incident ID number if there were multiple victims.
- WEAPON: Incident ID number and details about the weapon used (including weapons that were possessed by the shooter during the incident but were not fired). Multiple rows have the same incident ID number if there were multiple weapons used.

## Limitation
Due to my limited skill and expertise in data scraping, I couldn't find a way to automate the data scraping workflow on this dataset. My initial plan was like so in an attempt to create a dashboard out of it. I will leave that as a room for improvement for you.
