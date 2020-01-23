
# ETL And Analyze Amazon Cloud Review Data

This project used <span style="color:purple;">**PySpark**</span> and <span style="color:purple;">**AWS RDS**</span> do cloud data ETL. First creating tables based on review data's structure in *AWS RDS PostgreSQL* instance then within *ZELP notebook* environment using *PySpark* to *Extract* Amazon review dataset from *AWS S3 bucket* into PySpark dataframe then *Transform* the dataset and *Load* the DataFrames into the *AWS RDS PostgreSQL* instance. Last investigating whether Vine reviews are free of bias using *PySpark*.

- - -

![AmazonReview.jpg](assets/image1.png)

- - -


## Data source  

* Two datasets 'Software' and 'VideoDVD' are selected from  [**Amazon Review Datasets**](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt). 


## Technologies Used

*  **PySpark**:  Spark is a distributed computing framework and PySpark is the Python API for Spark a utility for spark python big data processing. The PySpark shell is responsible for linking the python API to the spark core and initializing the spark context. 

*  **ZEPL notebook**: ZEPL notebook is a completely open web-based notebook that enables interactive data analytics on Zepl which is the data science and analytics platform. 

*  **AWS RDS**: Amazon Relational Database Service (Amazon RDS) is a managed SQL database service provided by Amazon Web Services (AWS). Amazon RDS supports an array of database engines to store and organize data and helps with database management tasks, such as migration, backup, recovery and patching. 

*  **AWS S3**: Amazon Simple Storage Service(Amazon S3) is a service offered by Amazon Web Services(AWS) that provides object storage through a web service interface.   


## Project Files:

* **ETLAndAnalyzeAmazonReviewData.json**: This is the `ZEPL notebook` file. It connects to and loads in datasets from `AWS S3 bucket` to dataframes using `pyspark`, matched dataframe column types with the database column types and pushed final dataframes to `AWS RDS PostgreSQL`. And also analyzed whether reviews from Amazon's Vine program are trustworthy.



## Final Results

By running the ZEPL notebook can get below results: 

- - -

![result_1.png](static/images/12run.gif)


- - -
