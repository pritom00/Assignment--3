# Assignment--3
# Football Ticket Booking System

A complete Database Design and SQL implementation for a Football Ticket Booking System.

## 📋 Project Overview

This project demonstrates the design and implementation of a relational database for a Football Ticket Booking System. It includes proper table design, referential integrity, constraints, and advanced SQL queries.

## 🗃️ Database Schema

### Tables

- **Users** - Stores customer and admin information
- **Matches** - Contains football match details and ticket pricing
- **Bookings** - Records individual ticket bookings

### Entity Relationship Diagram




**Relationships:**
- One User → Many Bookings (**1:N**)
- One Match → Many Bookings (**1:N**)

## 🛠️ Technologies Used

- **Database**: PostgreSQL
- **SQL Features**: 
  - Primary Keys, Foreign Keys
  - Check Constraints
  - JOINs (INNER, LEFT)
  - Subqueries
  - Aggregate Functions
  - Pattern Matching (`ILIKE`)
  - NULL Handling (`COALESCE`)

## 📁 Files Included

- `QUERY.sql` - Complete DDL, Data Seeding & All Queries
- `ERD.JPG` - Entity Relationship Diagram

## 🚀 Database Setup

```sql
-- Run the full script in PostgreSQL
DROP TABLE IF EXISTS Bookings, Matches, Users;
-- (All CREATE TABLE, INSERT, and Queries)
Query Test CasesQuery 1: Champions League Available MatchesExpected Output:Real Madrid vs Barcelona (150.00)
Bayern Munich vs PSG (130.00)

Query 2: User SearchExpected Output:Tanvir Rahman
Asif Haque

Query 3: NULL Payment StatusExpected Output: Booking 504 with "Action Required"Query 4: Booking Details with JOINExpected Output: 5 booking records with user names and match fixturesQuery 5: All Users with LEFT JOINExpected Output: All 4 users (including Jannat Ara with NULL booking)Query 6: Above Average CostExpected Output: 3 bookings with cost 150.00Query 7: Top 2 Expensive Matches (with OFFSET)Expected Output: Bayern Munich vs PSG (130)
Man City vs Liverpool (120)

 Key Features Implemented Proper normalization (3NF)
 Referential Integrity using Foreign Keys
 Check constraints for data validation
 Support for NULL values
 Advanced SQL queries (JOIN, Subquery, Pagination)


