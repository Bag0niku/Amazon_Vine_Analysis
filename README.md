# Amazon_Vine_Analysis

The Amazon Vine program allows manufacturers to pay a fee and provide products to Amazon Vine members in exchange for reviews. The purpose of this project is to determine if there is a favorable bias in those Vine reviews.


## Tools:
 - Google Colabratory
 - Amazon Web Services (AWS)
 - pgAdmin 4, PostgresSQL 13.7
 - Datasource: Video Game Reviews from <a href="https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt">Amazon Reviews Datasets</a>

## Overview 
Amazon_Reviews_ETL.ipynb was written in Google Colab with PySpark. Amazon data was first loaded to a Spark DataFrame, then transformed to match schema set up by pgAdmin, and finally written to the RDS instance on AWS.     
    
Vine_Review_Analysis.ipynb was also written in Google Colab with PySpark. After data was retrieved from the SQL Database and converted to a spark dataframe, it was transformed to keep relevant columns, filtered, and analyzed to calculate the percentage of vine vs non-vine reviews. 

