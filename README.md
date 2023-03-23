# Crowdfunding_ETL
ETL is a type of data integration that refers to the three steps (extract, transform, load) used to
blend data from multiple sources. It's often used to build a data warehouse. During this process, 
data is taken (extracted) from a source system, converted (transformed) into a format that can be 
analyzed, and stored (loaded) into a data warehouse or other system. Extract, load, transform (ELT) 
is an alternate but related approach designed to push processing down to the database for improved 
performance. 

For Project 2 we first used ETL to extract and transform the Crowdfunding Excel data to create the 
category and subcategory dataframes. We also exported both dataframes as CSV files and saved it to our Github repository

![image](https://user-images.githubusercontent.com/119881903/227382913-7abfc22d-6668-43e6-8de0-c823597c6322.png)
![image](https://user-images.githubusercontent.com/119881903/227382991-967da422-c2d6-4fdc-b9bc-1c7402b79cb5.png)

We then extracted and transformed the Crowdfunding Excel data to create a campaign DataFrame
that includes all of the columns in the picture below. We also exported the campaign dataframe as a CSV and saved it to our Github repository.
![image](https://user-images.githubusercontent.com/119881903/227383349-038262e4-d867-45a3-ae81-c0aae95d8e76.png)

Next we extracted and transformed the data from the Contacts Excel data using Python dictionary methods. We then created a new dataframe that contains the extracted data and
split each "name" column value into a first and last name, and place each in a new column.
After that we cleaned and exported the contacts exceldata as a CSV file and saved it to our repository.
![image](https://user-images.githubusercontent.com/119881903/227383998-ccd198fe-92c1-4f69-83ba-361792c95c49.png)

Finally we created the Crowdfunding database. We started this process by sketching an ERD using QuickDBD. We then used this info to create a table shcema for each CSV file. Next we created a new Postgres database, named crowdfunding_db. Using the database schema, created the tables in the correct order to handle each foreign key. Finally we imported each CSV file into its corresponding SQL table and verified that each table has the correct data by running a SELECT statement for each.

The order for PGAdmin is CREATE TABLE "contacts", CREATE TABLE "campaign", CREATE TABLE "category",
CREATE TABLE "subcategory"

Validation Queries order
SELECT *
FROM public.contacts;

SELECT *
FROM public.campaign;

SELECT *
FROM public.category;

SELECT *
FROM public.subcategory;

ERD SKETCH

![image](https://user-images.githubusercontent.com/119881903/227384766-82d52f0a-1566-4f52-9205-35da5277f289.png)


