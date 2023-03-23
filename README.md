# Crowdfunding_ETL

## Background
For the ETL mini project, you will work with a partner to practice building an ETL pipeline using Python, Pandas, and either Python dictionary methods or regular expressions to extract and transform the data. After you transform the data, you'll create four CSV files and use the CSV file data to create an ERD and a table schema. Finally, you’ll upload the CSV file data into a Postgres database.

Since this is a one-week project, make sure that you have done at least half of your project before the third day of class to stay on track.

Although you and your partner will divide the work, it’s essential to collaborate and communicate while working on different parts of the project. Be sure to check in with your partner regularly and offer support.

## Instructions
The instructions for this mini project are divided into the following subsections:

* Create the Category and Subcategory DataFrames
* Create the Campaign DataFrame
* Create the Contacts DataFrame
* Create the Crowdfunding Database
### Create the Category and Subcategory DataFrames
1. Extract and transform the ```crowdfunding.xlsx``` Excel data to create a category DataFrame that has the following columns:

   * A "category_id" column that has entries going sequentially from "cat1" to "catn", where n is the number of unique categories

   * A "category" column that contains only the category titles

2. Export the category DataFrame as ```category.csv``` and save it to your GitHub repository.

3. Extract and transform the ```crowdfunding.xlsx``` Excel data to create a subcategory DataFrame that has the following columns:

   * A "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn", where n is the number of unique subcategories

   * A "subcategory" column that contains only the subcategory titles

4. Export the subcategory DataFrame as subcategory.csv and save it to your GitHub repository.
