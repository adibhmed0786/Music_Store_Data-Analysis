# Music Store Data Analysis (SQL Project)

This project analyzes a digital music store database using SQL to answer business-focused questions about customers, sales, genres, artists, and tracks.

## Project Objective

Use SQL queries to extract actionable insights from transactional music store data, such as:
- Top customers and spending behavior
- Best-performing cities/countries
- Most popular genres, artists, and songs
- Country-level customer trends

## Repository Contents

- `Music_Store_database.sql`  
  PostgreSQL database dump containing schema + data.
- `music_store.sql`  
  SQL analysis queries (15 questions and solutions).
- `music_store_erd.jpg`  
  Entity Relationship Diagram (ERD) of the database.

## Database Overview

The dataset includes key tables commonly found in a music-store system:
- `customer`, `employee`
- `invoice`, `invoice_line`
- `track`, `album`, `artist`, `genre`, `media_type`
- `playlist`, `playlist_track`

These tables support analysis across sales, catalog, and customer dimensions.

## Analysis Questions Covered

The `music_store.sql` file answers:
1. Senior-most employee by job level
2. Countries with the most invoices
3. Top 3 invoice totals
4. City with highest revenue
5. Best customer by total spend
6. Rock music listeners (customer list)
7. Top 10 rock artists by song count
8. Tracks longer than average song length
9. Customer spend by artist
10. Most popular genre per country
11. Top-spending customer per country
12. Most popular artists overall
13. Most popular songs overall
14. Average spend by genre
15. Countries with highest music purchases

## How to Run This Project

### 1) Prepare PostgreSQL
Install PostgreSQL and make sure `psql` and `pg_restore` are available.

### 2) Create Database
```bash
createdb music_database
```

### 3) Restore the Provided Dump
```bash
pg_restore -d music_database Music_Store_database.sql
```

### 4) Execute Analysis Queries
Run queries from `music_store.sql` using your SQL client, or with:
```bash
psql -d music_database -f music_store.sql
```

## Skills Demonstrated

- SQL Joins (INNER JOIN)
- Aggregation (`COUNT`, `SUM`, `AVG`)
- Grouping and sorting (`GROUP BY`, `ORDER BY`)
- Common Table Expressions (CTEs)
- Window functions (`ROW_NUMBER() OVER (...)`)
- Subqueries

## Suggested Improvements

- Add output snapshots/tables for each question
- Add query performance notes with indexing suggestions
- Add dashboard layer (Power BI/Tableau) for visualization

## Author

Project by repository owner/contributor of **adibhmed0786/Music_Store_Data-Analysis**.
