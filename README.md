# Load song details and song metatdata from files.
This project is to load the data of songs and listening log from files to a postgres db.
# Tools/Technologies used:
* Database: postgres
* Language: Python 3.x, SQL

# Prerequisites
1. Install python 3.x, postgres.
2. Clone this repository.
3. Run create_tables.py to create schema for the data.
4. Run etl.py to load data from files to the database.

# Files in the repo
1. `datasets.zip` contains example data loaded in this pipeline.
2. `create_tables.py` contains code to setup database and required tables taking the queries from `sql_queries.py`.
3. `etl.py` holds the flow of control and is entry point.
4. `sql_queries.py` holds SQL statements to create all the necessary tables and also the insert statements.
4. `*.ipynb` files are jupytor notebooks and were used to do trial runs before putting all the code in etl.py

# After running the code your database should have below tables with data.
1. artists  
2. songplays
3. songs
4. time
5. users