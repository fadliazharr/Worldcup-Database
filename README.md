# World Cup Database Project

## Overview
This project is a simple database implementation to store and query World Cup game data, specifically focusing on the final three rounds of the World Cup tournaments from 2014 onwards. The database contains information about teams, games, and scores. It allows querying various statistics, such as the total number of goals scored, the most goals scored in a single game, and the winner of the 2018 World Cup tournament.

## Purpose
The goal of this project was to create a database and populate it with game data from the World Cup, then use SQL queries to extract meaningful insights. The project uses a combination of shell scripts and PostgreSQL queries to achieve this.

## How It Works
1. **Database Structure**: 
   - A `teams` table is created with unique team names.
   - A `games` table stores game data, including the year, round, winner, opponent, and goals scored.
   
2. **Data Insertion**:
   - The `insert_data.sh` script is responsible for reading data from a CSV file (`games.csv`) and inserting the relevant information into the `teams` and `games` tables. The script ensures that each team is added only once.

3. **Queries**:
   - The `queries.sh` script executes various SQL queries to calculate statistics like the total number of goals, the average goals, the most goals scored in a game, and other related queries.
   
4. **Output**:
   - The results from the queries are printed to the console, including a list of teams that played in a specific round or a summary of goals scored in all games.

## Tools Used
- **PostgreSQL**: The database management system used to store and query the World Cup data.
- **Bash**: The shell scripting language used for writing the data insertion and querying scripts (`insert_data.sh` and `queries.sh`).
- **CSV**: Data from `games.csv` is processed and inserted into the database.

