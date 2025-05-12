# RR-RDB-Assessment
# SQL Queries for Codecademy Learners Data

This project analyzes mockup Codecademy learners data using SQL. Unlike traditional step-by-step tutorials, this project provides open-ended requirements that allow for flexibility in solving them. The goal is to explore different possible solutions using SQL queries, aggregate functions, and table joins. You will use the data from two tables: `users` and `progress`.

## Project Overview

This project allows you to use your SQL skills to explore the following:

- Analyzing `.edu` domains to find the top 25 schools.
- Querying how many `.edu` learners are from specific cities.
- Investigating users who use mobile apps and how that relates to their data.
- Analyzing learners' progress on various Codecademy courses.

The project does not provide a tutorial but instead offers requirements and open-ended tasks for you to solve using your knowledge of SQL.

## Tables

### Users Table:
- `user_id`: Unique identifier for each user.
- `email_domain`: Domain of the user's email.
- `country`: Country where the user is located.
- `postal`: Postal code.
- `mobile_app`: Indicates whether the user uses the mobile app (`mobile-user` or `NULL`).
- `sign_up_at`: The date and time the user signed up.

### Progress Table:
- `user_id`: Unique identifier for each user (related to `user_id` in `users`).
- `learn_cpp`: Indicates whether the user is progressing in learning C++.
- `learn_sql`: Indicates whether the user is progressing in learning SQL.
- `learn_html`: Indicates whether the user is progressing in learning HTML.
- `learn_javascript`: Indicates whether the user is progressing in learning JavaScript.
- `learn_java`: Indicates whether the user is progressing in learning Java.

## Project Goals

The goal of this project is to analyze the Codecademy learners' data with SQL by performing the following tasks:

1. **Explore the data**:  
   - Query all data from the `users` and `progress` tables to understand the structure.
   - Identify the top 25 `.edu` domains.

2. **Sign-Up Analysis**:
   - Use the `strftime()` function to analyze the sign-up times of users and group them by hour.

3. **Mobile App Usage**:
   - Determine how many learners are using the mobile app by analyzing the `mobile_app` column.

4. **Course Preferences**:
   - Investigate which courses are more popular among users from specific schools (i.e., `.edu` domains).
   - Analyze the courses that learners in New York and Chicago are taking.

## Setup Instructions

### Prerequisites:
- Familiarity with SQL, aggregate functions, and joining multiple tables.
- You should have completed the "Analyze Data with SQL" course or have equivalent experience.

### To run this project on your computer:

1. **Download SQLite**: If you don’t have it already, you can download SQLite from [SQLite's official website](https://www.sqlite.org/download.html).
2. **Install DB Browser**: Alternatively, you can use DB Browser for SQLite for a more user-friendly interface. [Download DB Browser](https://sqlitebrowser.org/).
3. **Setup Database**: Download the database file that contains the `users` and `progress` tables (or create it yourself with the appropriate schema).
4. **Run SQL Queries**: Open the `queries.sql` file in DB Browser or use the SQLite terminal to run the SQL commands.

### Tasks to Complete:

1. **Explore the data**:
   - Use `SELECT *` on both the `users` and `progress` tables to understand the data structure.
   - Query the top 25 `.edu` domains and analyze sign-up information.

2. **Sign-Up Analysis**:
   - Use the `strftime()` function to analyze sign-up times and group them by hour.

3. **Mobile App Usage**:
   - Count the number of learners using the mobile app from the `mobile_app` column.

4. **Course Analysis**:
   - Join the two tables and find out which courses are popular among learners from `.edu` domains.
   - Investigate the course preferences of learners in New York and Chicago.
