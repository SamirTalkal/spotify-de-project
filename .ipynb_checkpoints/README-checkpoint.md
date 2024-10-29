# Spotify Data Engineering Project

### Introduction
ETL Pipeline using Spotify API on AWS. The pipeline will retrieve data from the Spotify API, transform it to the desired format, and load it into an AWS data store.

### About Dataset/API
This API contains information about music artists, albums, and songs. - [Spotify API](https://developer.spotify.com/documentation/web-api)

### Services Used
1. S3
2. AWS Lambda
3. Cloud Watch
4. Glue Crawler
5. Data Catalog
6. Amazon Athena

### Installed packages
```
pip install pandas
pip install numpy
pip install spotipy
```

### Project Execution Flow
Extract Data from API -> Lambda Trigger (every 1 hour) -> Run extract Code -> Store Raw Data -> Trigger Transform Function -> Transform Data and Load It -> Query Athena Data
