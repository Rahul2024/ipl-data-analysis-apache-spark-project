<h1>IPL Data Analysis Project</h1>

This project is an in-depth analysis of Indian Premier League (IPL) data using Apache Spark. The aim is to derive meaningful insights from the rich dataset, including player performances, team statistics, and match outcomes. The analysis is performed using PySpark, making use of Spark’s powerful data processing capabilities to handle large datasets efficiently.
 
<h3>Project Overview</h3>
<h4>Objectives</h4>
1-Data Ingestion: Load IPL match data from CSV files stored in Amazon S3.
<br>
2-Data Transformation: Clean and preprocess the data using PySpark DataFrame operations.
<br>
3-Data Analysis: Perform various analyses such as top-scoring batsmen per season, economical bowlers in powerplay overs, and the impact of toss on match outcomes.
<br>
4-Visualization: Utilize the processed data for generating insights and visualizations (future scope).
<br>
<h3>Key Features</h3>
1-Data Schema Definition: StructType schemas defined for Ball_by_Ball, Match, Player, Player_Match, and Team datasets to ensure data integrity.<br>
2*Data Filtering: Filtered out extras like wides and no-balls for specific analyses.<br>
3-Aggregation & Window Functions: Used for calculating totals, averages, and running totals within a match.<br>
4-Conditional Columns: Created columns for high-impact balls and win margin categories.<br>
5-SQL Queries: Leveraged Spark SQL to perform complex queries for in-depth analysis.<br>
<h3>Technologies Used</h3>
Apache Spark: For distributed data processing.<br>
PySpark: Python API for Spark for writing Spark applications.<br>
Amazon S3: Cloud storage for storing and retrieving IPL datasets.<br>
Databricks: Cloud-based platform for running Spark jobs.<br>
<h3>Dataset</h3>
The IPL data consists of multiple CSV files stored in Amazon S3:<br>

Ball_By_Ball.csv: Detailed ball-by-ball information for each match.<br>
Match.csv: Metadata about each match including teams, venue, and results.<br>
Player.csv: Information about players, including their playing style.<br>
Player_match.csv: Player-specific performance data for each match.<br>
Team.csv: Basic details about the teams.<br>

<h3>How to Run</h3>
Setup the Environment:<br>

Install Apache Spark and PySpark.
Ensure you have access to the IPL dataset stored in Amazon S3.<br>
Run the Code:<br>

Start a Spark session.
Load the datasets into Spark DataFrames.
Perform data transformations and analyses as per the provided code.<br>
Analyze Results:<br>

Query the transformed data using Spark SQL.
Explore the insights generated, such as top batsmen, economical bowlers, and toss impact.
