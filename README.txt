# Final-Project-Transforming-and-Analyzing-Data-with-SQL

## Project/Goals
(fill in your description and goals here)
The goal of the project was to analyse and derive meaningful insights 
from an ecommerce database using postgresql
-In order to understand site visitors behaviour: Analyze the database to gain 
 insights into customer behavior, preferences, and purchase patterns.
-In order to segment the visitors based on their regions
-To identify marketing trends: Monitor market trends, industry developments, 
 and consumer preferences
-To assess Product performance: Evaluate the performance of individual 
 products or product categories based on orders, sales, revenue and region. 
-Geographic analysis: Evaluate sales performance and customer behavior across 
 different geographic regions or cities.



#Process
### The data based was imported manually into pgadmin, using character varying
as the default data type

### The data types of the tables were altered using the alter function, assigning
the correct data type to each column to ensure:
-Data Integrity
-Best query performance
-Better data presentation
-Easier Data manipulation

### To clean the data without altering the raw data values, sub tables were created
using CREATE TABLE function. The new tables were uniquely suffixed with "temp" to
avoid confusion.

### The new tables contained the clean data set
-Duplicate columns removed
-Redundant columns removed
-Corrected column names (e.g from v2productcategory to productcategory)
-Nulls removed
-Columns that had scanty values were removed
-Ajusting the values of the unit price (i.e unitprice/1,000,000)

### The new tables were used to answer all questions in the #Questions.txt#,
to form more questions #starting with questions# and a Quality Assurance process
was carried out and validated.

### ERD was generated based on the new tables created in pgadmin.



## Results
(fill in what you discovered this data could tell you and how you 
used the data to answer those questions)

The data can yield several valuable insights among them are;
-The most effective channel groups each visitor used to order products
-Detecting visitors that spent more than 2 hours on the site
-The dates with the most orders
-The city/country that had more visitors to place an order
-The transaction revenue generated
-The total revenue generated
-The most ordered products category
-The hierarchical pattern in the types of products ordered from
  each city

To get answers to the questions, it was necesary to; 
-Join tables
-Use subqueries and CTEs to reduce complexibilty of the queries
-Filter columns where necessary by using the WHERE operations
-Use Windowfunctions and GROUP BY to group columns
-And ORDER-ing the columns to fit the answers to the questions


## Challenges 
(discuss challenges you faced in the project)

-There were lots of duplicate and redundant columns
-The tables were unstable
-Limited number of days

## Future Goals
(what would you do if you had more time?)
-To derive more business insights from the database
-To carry out more quality assurance processes and validate the data
-To create a visualize representation of the data results


