# Crowdfunding_ETL Challenge

The purpose of this repository is to demonstrate the process of ETL (Extraction-Transformation-Loading) on a simple data set.
We were given two excel files contacts.xlsx and crowdfunding.xlsx from which we created 4 cleaned data sets, category.csv,
subcategory.csv, contacts.csv and campaign.csv which we then loaded to an sql database.

<img width="515" alt="Screen Shot 2023-08-23 at 12 49 12 pm" src="https://github.com/JackHast/Crowdfunding_ETL/assets/131254350/bdadb0ff-530d-4eca-87a4-fa73b770ce3d">

# Contents of Repository

This repository contains two jupyter notebooks ETL_Mini_Project.ipynb and to_sql.ipynb. There are 4 csv files created from ETL_Mini_Project.ipynb
which are located in the folder Resources along with the two excel files contacts.xlsx and crowdfunding.xlsx that were provided. Finally, there is an sql file provided, 
crowdfunding_db_schema.sql, which contains the schemas for the tables required in to_sql.ipynb.

# Instructions

The jupyter notebook ETL_Mini_Project.ipynb can be run using jupyter or VScode as long as numpy and pandas are installed.
In order for to_sql.ipynb to run on your local computer, sqlalchemy and psycopg2 must be installed and a database 'crowdfunding_db' 
must be created using Postgresql from which crowdfunding_db_schema.sql needs to be run to create the 4 empty tables. to_sql.ipynb will
connect to 'crowdfunding_db' and then append the dataframes 'categories_df', 'subcategories_df', 'contacts_df' and 'campaign_df' to the corresponding
tables.
In order for the notebook to connect with the database you've created you need to enter your Postgresql username, password and port in to_sql.ipynb,

<img width="864" alt="Screen Shot 2023-08-23 at 6 51 55 pm" src="https://github.com/JackHast/Crowdfunding_ETL/assets/131254350/1f40e386-1881-4323-a05a-ea0eabd4e686">

The required libraries can be installed in your environment by running the following in your terminal/command-line,

pip install pandas <br>
pip install numpy <br>
pip install sqlalchemy <br>
pip install psycopg2


# Acknowledgements

The first section of ETL_Mini_Project.ipynb which creates the category and subcategory csv's was done by Andrew Mclaughlin,
the second section which creates the campaign csv was created by Raviska and the code that creates the cleaned contacts csv was done by Jack Hastings. 
The sql file crowdfunding_db_schema.sql was done by Andrew Mclaughlin who used QuickDBD.com to create the ERD shown above.
For the jupyter notebook, ETL_Mini_Project.ipynb starter code was provided by the Monash Data Analytics Bootcamp: https://bootcamps.monash.edu/data/.
 



