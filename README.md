IPL Data Analysis Project
This project is an in-depth analysis of Indian Premier League (IPL) data using Apache Spark. The aim is to derive meaningful insights from the rich dataset, including player performances, team statistics, and match outcomes. The analysis is performed using PySpark, making use of Spark’s powerful data processing capabilities to handle large datasets efficiently.

Project Overview
Objectives
Data Ingestion: Load IPL match data from CSV files stored in Amazon S3.
Data Transformation: Clean and preprocess the data using PySpark DataFrame operations.
Data Analysis: Perform various analyses such as top-scoring batsmen per season, economical bowlers in powerplay overs, and the impact of toss on match outcomes.

Visualization: Utilize the processed data for generating insights and visualizations (future scope).
Key Features
Data Schema Definition: StructType schemas defined for Ball_by_Ball, Match, Player, Player_Match, and Team datasets to ensure data integrity.
Data Filtering: Filtered out extras like wides and no-balls for specific analyses.
Aggregation & Window Functions: Used for calculating totals, averages, and running totals within a match.
Conditional Columns: Created columns for high-impact balls and win margin categories.
SQL Queries: Leveraged Spark SQL to perform complex queries for in-depth analysis.
Technologies Used
Apache Spark: For distributed data processing.
PySpark: Python API for Spark for writing Spark applications.
Amazon S3: Cloud storage for storing and retrieving IPL datasets.
Databricks: Cloud-based platform for running Spark jobs.
Dataset
The IPL data consists of multiple CSV files stored in Amazon S3:

Ball_By_Ball.csv: Detailed ball-by-ball information for each match.
Match.csv: Metadata about each match including teams, venue, and results.
Player.csv: Information about players, including their playing style.
Player_match.csv: Player-specific performance data for each match.
Team.csv: Basic details about the teams.
How to Run
Setup the Environment:

Install Apache Spark and PySpark.
Ensure you have access to the IPL dataset stored in Amazon S3.
Run the Code:

Start a Spark session.
Load the datasets into Spark DataFrames.
Perform data transformations and analyses as per the provided code.
Analyze Results:

Query the transformed data using Spark SQL.
Explore the insights generated, such as top batsmen, economical bowlers, and toss impact.
