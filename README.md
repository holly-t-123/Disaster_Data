# Disaster_Data

EDA process:
I was already relatively familar with this data. The biggest issue was how different the datasets were from one to the next. I needed to figure out how to extract the useful information in a way that would work for every data set, while keeping the PII separate yet indexable from the main data set I needed to create: contact points.

ETL process:

Excel (choosing columns, removing PII from notes, converting to csv, replacing values that I knew would cause problems such as apartment hyphens)

Python (Specifying dtypes for the columns I would use, fill null values and dropping duplicates, creating a mask to iterate through relevant rows, creating functions to extract survivors, residences, and contact points into separate data frames)