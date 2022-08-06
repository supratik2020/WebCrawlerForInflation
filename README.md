# Table of Contents 
1. [Introduction](README.md#introduction)
2. [Pipeline](README.md#pipeline)
3. [Requirements](README.md#requirements)
4. [Environment Set Up](README.md#Environment%20Setup)
5. [Repository Structure and Run Instructions](README.md#Repository%20Structure%20and%20Run%20Instructions)


# Introduction
**Price Crawler: Tracking Price Inflation**

 A sample batch job has 
been executed using online laptop prices ($500-$800) and the inflation rate in 2019 is measured to be 4.8% which is more than double the annual inflation rate of 
2.3% reported by Bureau of labor statistics for 2019.  

# Pipeline
I built a data pipeline that utilizes petabytes of publicly available web page data to **Calculate Inflation rates from first principles (Prices of Products)**



1. AWS Athena to query indexed WARC Files using HTTP header information in WARC Files
    * Scan 0(100 GB) data instead of PB
2. **Keys** to webpages of interest saved in parquet files on S3
3. Parquet + WARC input to Spark with distributed processing over O(10 GB) data per job
4. Cleaning, filtering and aggregating Product and Price tables with Pandas in Python
5. Plotting and tracking price trends with Dash

**Languages** 
* Bash
* Python 3.7
* Pandas

**Technologies**
* Spark
* AWS Athena
* Dash/Plotly

**Third-Party Libraries**
* AWS CLI


Technologies

* Amazon DynamoDB

