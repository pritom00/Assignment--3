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

![ERD](erd.png)  
*(Replace with your actual ERD image or link)*

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
- `ERD.png` - Entity Relationship Diagram

## 🚀 Database Setup

```sql
-- Run the full script in PostgreSQL
DROP TABLE IF EXISTS Bookings, Matches, Users;
-- (All CREATE TABLE, INSERT, and Queries)
