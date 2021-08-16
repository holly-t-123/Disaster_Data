# Disaster_Data

I worked with Hands On Nashville when they activated Disaster Response Mode for the March 2021 flooding in South Nashville. As part of the data team, I helped collect, process, and analyze the survivor data that came in from a number of different sources. The process was very manual and relied on a lot of copy-pasting between Excel spreadsheets. I decided to use this data for my Data Analytics Capstone project and applied my new skills to the same data set to increase both the efficiency and functionality of the analysis.

EDA process:
I was already relatively familar with this data. The biggest issue was how different the datasets were from one to the next. I needed to figure out how to extract the useful information in a way that would work for every data set, while keeping the Personally Identifiable Information (PII) separate yet indexable from the main data set I needed to create: contact points. Below you can see the column headers from each of the data sets I was working with...

![raw data](images/raw_data_headers.png)


ETL process:

Excel (choosing columns, removing PII from notes, converting to csv, replacing values that I knew would cause problems such as apartment hyphens)

Python (Specifying dtypes for the columns I would use, fill null values and dropping duplicates, creating a mask to iterate through relevant rows, creating functions to extract survivors, residences, and contact points into separate data frames)