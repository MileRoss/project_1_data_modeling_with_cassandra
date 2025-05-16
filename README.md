
# Project: Data Modeling with Cassandra

## Project Overview
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data, since the data reside in a directory of CSV files.  

They'd like a data engineer to create an Apache Cassandra database to query song play data and answer specific questions. Your role is to create this database. You'll be able to test it by running queries provided by the analytics team.

## Project Details

### Datasets
You will work with one dataset: `event_data`. It contains CSV files partitioned by date, such as:
- `event_data/2018-11-08-events.csv`
- `event_data/2018-11-09-events.csv`

### Project Template
You are provided with a Jupyter Notebook template that:
- Processes the `event_datafile_new.csv` to create a denormalized dataset
- Helps model the data tables based on required queries
- Loads the data into Apache Cassandra tables and runs queries

## Project Steps

### Modeling your NoSQL database
- Design tables for the queries
- Write `CREATE KEYSPACE` and `SET KEYSPACE`
- Use `CREATE TABLE IF NOT EXISTS` and `DROP TABLE IF EXISTS`
- Use appropriate `PRIMARY KEY` with partition and clustering columns
- Run `SELECT` queries to test

### Build ETL Pipeline
- In Part I, process each CSV file and output a new CSV: `event_datafile_new.csv`
- In Part II, use `CREATE` and `INSERT` statements to load data into Cassandra
- Run `SELECT` queries to verify

## Project Requirements

### ETL Pipeline Processing
- Complete the ETL pipeline
- Create `event_datafile_new.csv`
- Use correct datatypes in `CREATE` statements

### Data Modeling
- Build accurate data models
- Use appropriate table names and column order
- Ensure queries return correct results without `ALLOW FILTERING`

### PRIMARY KEYS
- Use partition keys and clustering columns to uniquely identify rows

### Presentation
- Include explanations of queries
- Clean and modular code
- Remove in-line instructions meant only for you

## Suggestions to Stand Out
- Describe your PRIMARY KEY choices
- Use pandas DataFrames for better output readability
