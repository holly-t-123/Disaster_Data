# Disaster_Data

-Intro
-

I worked with Hands On Nashville when they activated Disaster Response Mode for the March 2021 flooding in South Nashville. As part of the data team, I helped collect, process, and analyze the survivor data that came in from a number of different sources. The process was very manual and relied on a lot of copy-pasting between Excel spreadsheets. I decided to use this data for my Data Analytics Capstone project to apply my new skills to increase both the efficiency and functionality of the analysis.

Excel:

The main hurdle at first was cleaning the 10 different data sets. Below you can see the column headers copy-pasted from each file I was working with to get an idea of how varied they were...

![raw data](images/raw_data_headers.png)

Cleaning issues I had to solve included...
- No entry dates on most of the spreadsheets (Chose to give all entries the date that Hands On Nashville received the spreadsheet)
- Inconsistent address format (Pared everything down to Street Number, Street Name with no hyphens in apartments)
- PII in the comments (Scanned through to manually delete PII)
- Capitilization issues creating unnecessary categories (Simple replacement function)

Python:

I wanted a way to extract the data into related tables that masked the PII with numbered IDs. In order to streamline the process, I built three functions that would take in whatever information was available (which differed between data sets), account for duplication, and return relevant IDs to be used in the main table. Then I could use a standard format for passing each data set into the functions, changing file names and column names as needed. All of this code can be found in the "Creating Schema" notebook. I have included screenshots below to illustrate the functions, the template I used to parse each of the 10 files, and the resulting ERD. 

