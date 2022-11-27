# Crowdfunding-ETL
## Overview
   This project required the use of Python, Pandas, and Jupyter notebooks to extract and transform data, and SQL to update and load the transformed data into a database. The ETL process enabled the successful collection, cleaning, and storage of data, as well as some refined new analysis.
## Results
   Extracting and transforming the data required using Python methods, and I chose the dictionary method to create a new DataFrame that parsed the data into more readable and useable information. Upon completion of the *EXTRACT* and *TRANSFORM* phases, the new DataFrame was exported into the [backers](Resources/backers.csv) file use in the *LOAD* phase.
   
   The final [code](Extract-Transform_final_code.ipynb) demonstrates how I imported the appropriate dependencies, inspected the data, created the new DataFrame, cleaned the data, and exported the data into a new CSV file.
   
   For the *TRANSFORM* phase I created an [Entity Relationship Diagram](Resources/crowdfunding_db_relationships.png) to inform my [SQL code](Queries/crowdfunding_db_schema.sql) and the creation of useable tables in the database. After verifying the backers table successfully imported information from the backers.csv file, additional analysis allowed Independent Funding to refine their engagement strategy with their backers.
## Summary
   Analyzing the newly imported data allowed IF to give their backers email nudge to let them know how the live campaign they've funding is doing. This was possible becasue of how I executed the ETL process. A new [query](Queries/crowdfunding_SQL_Analysis.sql) consolidated the information management required to refine their communication strategy, and the [backers](Data/email_backers_remaining_goal_amount.csv) and [contacts](Data/email_contacts_remaining_goal_amount.csv) files were sent to the marketing department for follow-on engagments.
