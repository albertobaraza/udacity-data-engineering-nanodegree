# Data Engineering Nanodegree Program

This GitHub repository was made for completing all the projects needed to finish [this](https://www.udacity.com/course/data-engineer-nanodegree--nd027) Udacity course.

# Repository structure

In the repo, each directory represents a project (projects are ordered by submission time). Each directory has its own README, so please do not hesitate to check them for more detail.

## [Data Modeling with Postgres](https://github.com/albertobaraza/udacity-data-engineering-nanodegree/tree/master/Data%20Modeling%20with%20Postgres)

This project gives a good example on how to build, populate and test a relational database (DB) in Postgresql using [Jupyter notebooks][jp] and `psycopg2` as a DB adapter.

## [Data Modeling with Apache Cassandra](https://github.com/albertobaraza/udacity-data-engineering-nanodegree/tree/master/Data%20Modeling%20with%20Apache%20Cassandra)

In this project, we move from SQL to NoSQL using [Apache Cassandra](https://cassandra.apache.org/) as the datasource of the project. It was developed using [Jupyter notebooks][jp], `cassandra` as the DB adapter and **CQL** as the programming language beside python.

## [AWS Data Warehouse](https://github.com/albertobaraza/udacity-data-engineering-nanodegree/tree/master/AWS%20Data%20Warehouse)

A cloud data warehouse for the fictional music streaming company Sparkify. Raw event and song data is copied from S3 into staging tables on [Amazon Redshift](https://aws.amazon.com/redshift/), then transformed into a star schema (one `songplays` fact table and `users`, `time`, `artists` and `songs` dimension tables) using Python and `psycopg2`.

## [Data Lake with Spark](https://github.com/albertobaraza/udacity-data-engineering-nanodegree/tree/master/Data%20Lake%20with%20Spark)

The same Sparkify analytics use case, rebuilt as a data lake. [Apache Spark](https://spark.apache.org/) reads song and log JSON data directly from an S3 bucket, builds the same star schema in memory, and writes the resulting dimension and fact tables back out to S3 as partitioned Parquet files.

## [Data Pipelines with Airflow](https://github.com/albertobaraza/udacity-data-engineering-nanodegree/tree/master/Data%20Pipelines%20with%20Airflow)

Sparkify's ETL is orchestrated as an [Apache Airflow](https://airflow.apache.org/) DAG. Custom operators stage data from S3 into Redshift, load the fact and dimension tables, and run automated data quality checks, all scheduled and monitored from the Airflow UI.

## [Capstone project - Analytics in agriculture](https://github.com/albertobaraza/udacity-data-engineering-nanodegree/tree/master/Capstone%20project%20-%20Analytics%20in%20agriculture)

A capstone project analyzing global crop production and trade data from the [FAO](http://www.fao.org/faostat/en/). Raw CSV data (9M+ rows) is cleaned, split into a star schema, and loaded into Redshift via S3, with the results exposed through a [Power BI](https://powerbi.microsoft.com/) report. The README also discusses how the design would evolve to handle 100x data growth, a daily schedule, and 100+ concurrent users.

[jp]: https://jupyter.org/
