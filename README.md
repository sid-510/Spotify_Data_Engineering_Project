# Spotify End-to-End Pipeline Data Engineering Project

## Overview

In this End-to-End Data Engineering project I have used the Spotify API to extract details of the "Top Songs - Global" playlist, transform the album, artist and songs data and load it in Athena for analytics.

<img width="1153" alt="Screenshot 2023-06-22 at 7 23 46 PM" src="https://github.com/sid-510/Spotify_Data_Engineering_Project/assets/96101913/2094f9f8-c269-4512-84e9-a628493fed98">

## Project Goals
- Integrating with Spotify API and extracting Data
- Deploying code on AWS Lambda for Data Extraction
- Adding trigger to run the extraction automatically
- Writing transformation function
- Building automated trigger on transformation function
- Store files on S3 properly
- Building Analytics Tables on data files using Glue and Athena

## Architecture Diagram
![IMG_65305C82915A-1](https://github.com/sid-510/Spotify_Data_Engineering_Project/assets/96101913/bb25d491-d507-4c80-95a6-c2e14dabfbf0)

## Services used
1. AWS Lambda: Lambda is a computing service that allows programmers to run code without creating or managing servers.
2. Amazon S3: Amazon S3 is an object storage service that provides manufacturing scalability, data availability, security, and performance.
3. AWS Crawler: Crawler is used to populate the AWS Glue Data Catalog with tables. 
4. AWS Athena: Athena is an interactive query service for S3 in which there is no need to load data it stays in S3.

## API used

Used the Spotify API.

## Code

Have used the ``spotify_api_data_extract.py`` python code to extract the details using Spotify API.

Have used the ``spotify_transformation_load_function.py`` python code to transform the extracted information.
