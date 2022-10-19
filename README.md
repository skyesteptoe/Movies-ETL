# Extract, Transform, Load (ETL)
## An Aggregation of Movie Data

## Project Overview

### Background
This analysis required that we compile data from multiple places. Each dataset requires cleaning and structuring before it can be analyzed. The Extract, Transform, Load process breaks this process into three steps. The Extract step reads in data, often from various sources. The Transform step comes next and summarizes the data-cleaning step to ensure it is in an analyzable format. The final step is Load, where the data is written to a database for storage.

### Purpose
Amazing Prime, a streaming platform, has sponsored a hack-a-thon. They want to develop an algorithm to predict what low-budget movies will become popular. With that information, they will purchase the streaming rights. Hackers will be provided a clean data-set of movie data to get them started!

### Analysis Overview
This analysis process is broken down into four parts with jupyter notebooks linked below for each step.

Part 1. [ETL_function_test.ipynb](https://github.com/skyesteptoe/Movies-ETL/blob/main/ETL_function_test.ipynb)
- Data was extracted in JSON and CSV formats.
- Data was transformed into Pandas data frames

Part 2. [ETL_clean_wiki_movies.ipynb](https://github.com/skyesteptoe/Movies-ETL/blob/main/ETL_clean_wiki_movies.ipynb)
- Created a clean_movie function to combine movie data with alternative languages into one column called alt_titles.
- A subfunction, change_column, organized column names into a clearer order
- Used created function, extract_transform_load, to complete multiple transformation steps

Part 3. [ETL_clean_kaggle_data.ipynb](https://github.com/skyesteptoe/Movies-ETL/blob/main/ETL_clean_kaggle_data.ipynb)
- Used the extract_transform_load to clean the Kaggle data and merge dataframes.

Part 4. [ETL_create_database.ipynb](https://github.com/skyesteptoe/Movies-ETL/blob/main/ETL_create_database.ipynb)
- Connected to SQL database (Postgres), completing the ETL process.