# Data Cleaning Project — Database Schema

## Overview
This repository documents the MongoDB schema for our data-cleaning web application.

## Database
- **Database name:** `data_cleaning_db`
- **Database:** MongoDB Atlas

## Collections

### 1. users
Stores user account details.
- `name`: String
- `email`: String
- `created_at`: Date

### 2. jobs
Stores uploaded dataset and cleaning-job information.
- `user_id`: ObjectId
- `file_name`: String
- `file_type`: String
- `status`: String
- `created_at`: Date

### 3. cleaning_reports
Stores data-cleaning results.
- `job_id`: ObjectId
- `rows_before`: Integer
- `rows_after`: Integer
- `duplicates_removed`: Integer
- `missing_values_fixed`: Integer
- `created_at`: Date

## Validation
MongoDB JSON Schema validation rules have been configured in Atlas for all three collections.

## Files
- `database_schema.json` — documents the database and collection structure.
- `README.md` — explains the schema and collections.
