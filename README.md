## Project Scenario:
An international firm that is looking to expand its business in different countries across the world has recruited you. 

You have been hired as a junior Data Engineer and are tasked with creating an automated script that can extract the list of all countries in order of their GDPs in billion USDs (rounded to 2 decimal places), as logged by the International Monetary Fund (IMF). 

Since IMF releases this evaluation twice a year, this code will be used by the organization to extract the information as it is updated.

The required information needs to be made accessible as a CSV file Countries_by_GDP.csv as well as a table Countries_by_GDP in a database file World_Economies.db with attributes Country and GDP_USD_billion.

Your boss wants you to demonstrate the success of this code by running a query on the database table to display only the entries with more than a 100 billion USD economy. Also, you should log in a file with the entire process of execution named etl_project_log.txt.

You must create a Python code 'etl_project_gdp.py' that performs all the required tasks.

## Source
The required data seems to be available on the URL mentioned below:

'https://web.archive.org/web/20230902185326/https://en.wikipedia.org/wiki/List_of_countries_by_GDP_%28nominal%29'

## Objectives
You have to complete the following tasks for this project
- Write a data extraction function to retrieve the relevant information from the required URL.

- Transform the available GDP information into 'Billion USD' from 'Million USD'.

- Load the transformed information to the required CSV file and as a database file.

- Run the required query on the database.

- Log the progress of the code with appropriate timestamps.
  

## Initial setup
The libraries needed to run the script are as follows:

- requests - The library used for accessing the information from the URL.

- bs4 - The library containing the BeautifulSoup function used for webscraping.

- pandas - The library used for processing the extracted data, storing it to required formats and communicating with the databases.

- sqlite3 - The library required to create a database server connection.

- numpy - The library required for the mathematical rounding operation as required in the objectives.

- datetime - The library containing the function datetime used for extracting the timestamp for logging purposes.
